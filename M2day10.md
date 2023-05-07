# What is Wireless Network?

● A wireless network is a set of two or more devices connected 
with each other via radio waves within a limited space range. 

● The devices in a wireless network have the freedom to be in 
motion, but be in connection with the network 

● One of the most crucial point that they are so spread is that their 
installation cost is very cheap and fast than the wire networks.

● Wireless networks are widely used and it is quite easy to set 
them up. 

● A wireless router is the most important device in a wireless 
network that connects the users with the Internet.

# What is Wireless Hacking?

● Wireless hacking is essentially cracking the security protocols in a wireless 
network

● granting full access for the hacker to view, store, download, or abuse the 
wireless network.

● Usually, when someone hacks into a Wifi, they are able to observe all the data 
that is being sent via the network with MiTM attack.

● In a wireless network, we have Access Points(AP), A wireless access point (wireless AP) is a 
network device that transmits and receives data over a wireless local area network 
(WLAN), 

    ○ serving as the interconnection point between the WLAN and a fixed wire network.

    ○ Found inside the wireless router(we use in our house)

* …

● A hacker can sniff the network packets without having to be in the same 
building where the network is located. As wireless networks communicate 
through radio waves, a hacker can easily sniff the network from a nearby 
location.

● Most attackers use network sniffing to find the SSID and hack a wireless 
network.

● When our wireless cards are converted in sniffing modes, they are called 
monitor mode

● And when your Wireless card allows to configure a AP on your laptop manually it 
is called Managed mode

● TO do most wireless Hacking , you need a device that can intercept or handle 
that specific signal.

# Wifi Hacking

● For this we need a wifi Antenna for our Computer.

● Most Laptops Have A wireless card inside of them but the desktops doesn't have. That's 
why they don't get any wifi networks on desktop .

● But the Adapter Have to have a feature called “Packet Injection+monitor mode”.

● If you are on Virtual Machines You must need Adapters, if you are on Dual boot,main boot 
and live boot you are Good to go

# Wireless network Algorithms

● Terms

    ○ SSID/Service set Identifier/: it is just the name of the AP

    ○ BSSID/Basic Service Set Identifier/: Mac Address of the Wireless AP device.

    ○ WLAN: Wireless Local Area Network, same as wifi

    ○ Channel: are smaller bands within WiFi frequency bands that are used by your 
    wireless network to send and receive data. Depending on which frequency band 
    your router is using, you have a certain number of WiFi channels to choose from:

■ 13 WiFi channels are in the 2.4 GHz frequency band

■ 45 WiFi channels are in the 5 GHz frequency band

● WIreless Network algorithms are algorithms used on setting up our AP, that helps to 
secure the network.

● There are Four kinds of WLAN Security Algorithms

        ○ WEP

        ○ WPA

        ○ WPA2

        ○ WPA3

* WEP - Wired Equivalent Privacy

● WEP encrypts traffic using a 64- or 128-bit key in hexadecimal.

● This is a static key, which means all traffic, regardless of device, is encrypted 
using a single key. 

● A WEP key allows computers on a network to exchange encoded messages 
while hiding the messages' contents from intruders. 

● This key is what is used to connect to a wireless-security-enabled network.

● One of WEP’s main goals was to prevent Man-in-the-Middle attacks, which it did for a time. 

● However, despite revisions to the protocol and increased key size, various security flaws were 
discovered in the WEP standard over time. As computing power increased, it became easier to exploit 
for criminals to exploit those flaws. Because of its vulnerabilities, 

● the Wi-Fi Alliance officially retired WEP in 2004. Today, WEP security is considered obsolete, although it 
is still sometimes in use – either because network administrators haven’t changed the default security 
on their wireless routers or because devices are too old to support newer encryption methods like WPA.

* WPA - Wi-Fi Protected Access

● this protocol was the Wi-Fi Alliance’s replacement for WEP. 

● It shared similarities with WEP but offered improvements in how it handled security keys and the way users are 
authorized. 

● While WEP provides each authorized system with the same key, WPA uses the temporal key integrity protocol 
(TKIP), which dynamically changes the key that systems use. 

● WPA included message integrity checks to determine if an attacker had captured or altered data packets.

● The keys used by WPA were 256-bit, a significant increase over the 64 bit and 128-bit keys used in the WEP 
system.

● However, despite these improvements, elements of WPA came to be exploited – which led to WPA2.

● You sometimes hear the term ‘WPA key’ in relation to WPA. 

● A WPA key is a password that you use to connect to a wireless network. 

● You can get the WPA password from whoever runs the network. In some cases, a default WPA passphrase or 
password may be printed on a wireless router. If you can't determine the password on your router, you may be 
able to reset it.

* WPA2 - Wi-Fi Protected Access 2

● WPA2 operates on two modes:

    ○ Personal mode or Pre-shared Key (WPA2-PSK) – which relies on a shared passcode for 
    access and is usually used in home environments.

    ○ Enterprise mode (WPA2-EAP) – as the name suggests, this is more suited to organizational or 
    business use.

● Both modes use the CCMP – which stands for Counter Mode Cipher Block Chaining Message 
Authentication Code Protocol. The CCMP protocol is based on the Advanced Encryption Standard 
(AES) algorithm, which provides message authenticity and integrity verification. CCMP is stronger and 
more reliable than WPA's original Temporal Key Integrity Protocol (TKIP), making it more difficult for 
attackers to spot patterns.

● However, WPA2 still has drawbacks. For example, it is vulnerable to key reinstallation 
attacks (KRACK). 

● KRACK exploits a weakness in WPA2, which allows attackers to pose as a clone network
and force the victim to connect to a malicious network instead. 

● This enables the hacker to decrypt a small piece of data that may be aggregated to crack
the encryption key.

● However, devices can be patched, and WPA2 is still considered more secure than WEP or 
WPA.

* WPA3 - Wi-Fi Protected Access 3

● WPA3 introduced new features for both personal and enterprise use, including:

    ○ Individualized data encryption: When logging on to a public network, WPA3 
    signs up a new device through a process other than a shared password. 

■ WPA3 uses a Wi-Fi Device Provisioning Protocol (DPP) system that allows 
users to use Near Field Communication (NFC) tags or QR codes to allow 
devices on the network.

■ In addition, WPA3 security uses GCMP-256 encryption rather than the 
previously used 128-bit encryption.

    ○ Simultaneous Authentication of Equals protocol: 

■ This is used to create a secure handshake, where a network device will 
connect to a wireless access point, and both devices communicate to verify 
authentication and connection. 

■ Even if a user’s password is weak, WPA3 provides a more secure 
handshake using Wi-Fi DPP.

● WPA3 devices became widely available in 2019 and are backwards compatible with 
devices that use the WPA2 protocol.

# WLAN Recon

● For any wifi sniffing Activity our adapter have to be on 
sniffing mode, means Monitor mode.( Default is Managed 
Mode)

● To Check our adapters mode,

    Iwconfig

● To change it we will use a tool called “airodump-ng”

    airmon-ng start <inferface>

# Recon…

● On Wireless Networks, The informations we 
will gather are the following:

    SSID/ESSID

    BSSID

    Channel

    Algorithm

Manufacturer of the Router

● To get informations about our wifi

    airodump-ng <interface>

# Hacking WLAN

● Let’s see some Hacking methods for wifi networks.

    ○ WPS enabled

    ○ Handshake Bruteforce

    ○ WEP Attack

    ○ Evil-twin attack

1) WPS Enabled

● Wi-Fi Protected Setup (WPS) is a feature supplied with many routers. 

● It is designed to make the process of connecting to a secure wireless network 
from a computer or other device easier.

* HOW?

● WPS uses some 8 digit code to connect. And attackers will bruteforce this pin.

● There are many tools on linux to do this but the simples and easiest way it to use some 
android apps like:

Detail how to use it: 

        sudo reaver -i wlan0 -b <macaddress> -vv

    https://null-byte.wonderhowto.com/how-to/hack-wpa-wifi-passwords-by-cracking-wps-pin-01
    32542/

# Prevention ways.

● This is the most simples attack to do 
and Many script kiddies are into this.

● To prevent it, you just need to 
disable it from your router setting.

2) Handshake Bruteforce

● Handshake in wireless networks is the exchange 
of information between the access point and 
the client at the time the client connects to it. 

● This information contains a variety of keys, the 
exchange takes place in several stages.

● It is a 4-way handshake.

● By default, the network card listens only for the 
packets addressed to itself. The monitor mode 
enables the network card to listen to every packet in 
the air. Listening to all the packets can help the card 
capture the 4-way handshakes.

* …

● Hackers will try to kick a person from a wifi(called 
deauthentication) and sniff the network, when the 
user try to connect back, they will have the 
Handshake file.

● This file can be brute forced and got the right 
password.

● For this:

1. Get wifi info

2. Sniff on that wifi specific channel

3. Deauthenticate the wifi(on different shell)

4. Get the handshake

5. Crack it with aircrack.

* Sniffing to the network

● On this Step we will listen to specific 
channel of our Target.

    Channel: 4

● Syntax:

    airodump-ng <interface> –channel 

    <channel> -w <filename>

■ The -w means write it to a file.

* Deauth

● On another terminal, we will start a 
deauthentication attack.

● This will make our handshake capturing process 
quick.

● As we saw the handshake is captured when logged 
user try to connect to the network back.

● So we will forcely kick him and listen for 
handshakes on our other terminal.

● Syntax:

    aireplay-ng -0 <size> -a <MAC_o_target> 
    <interface>

■ -0 means how many times the deauth is sent.

■ -a is the attack target.

● What kind of attack do this look like?(well known)

# Capturing Handshake

● CONGRATULATIONS!

● We have Got the handshake!

● Now we need to crack it and get our Password.

● TO do this we will use a tool called 
“Aircrack-ng”

● This is done Because of Phones automatic 
connect try

- NOTE: The tools we saw(airmon,airodump,aireplay) 
all are in the package of aircrack-ng

    sudo apt install aircrack-ng

* Cracking

● On this step we will brute force the password and 
try to crack it.

● The time of the password gaining bases on the 
wordlist you have.

○ If you gathered and made your own Good wordlist 
you have a chance to get it.

● Syntax:

    aircrack-ng <cap_file> -w <wordlist>

# Prevention way

1. Using WPA3 which is a newer protocol is your best bet 
against such an attack.

2. To mitigate against de-authentication attacks

3. use an ethernet connection if possible.

4. use a strong passphrase (not a password) to minimise the 
attackers chances of getting it

a. Example: my home wifi password is something like: 
“Helloworldthisismypassword”

b. This will be very hard to crack it wordlist.

3) WEP attack

- The Steps are same with the 
Handshake bruteforce the 
difference is here we will 
bruteforce an encryption key 
not password.

- Also we don't capture 
handshake,we just listen for 
WEP wifi for some minutes.

- And we will crack it with 
aircrack-ng.

## Evil-twin Attack

● It is an amazing attack. It includes

a. Deauthentication,

b. Fake AP and 

c. phishing.

● The way it work is:

a. Attacker will clone one of the wifi he 
going to attack with making it open wifi

b. Then it will initiate deauth on real wifi, 
so users will be forced to be on the fake 
one.

c. Then the attacker will fake prompt to 
input the password to access the wifi
d. When the users add the password, 
BOOM! Attacker will have the 
password. 

● This is the most Effective way to hack a 
wifi.

● That is why the name is “Evil twin”

How?

- It have a lot of steps and it is 
complicated to do it manually, 
but there are a lot of tools to do 
it Automatically.

 Lets see the tool Airgeddon

- Link: 

        https://github.com/v1s1t0r1sh
        3r3/airgeddon

# Prevention

● Avoid Wi-Fi networks marked as “Unsecure”

● Use your own hotspot

● Disable Wi-Fi autosave

● Use a VPN

● Only browse HTTPS sites

# Bluetooth Hacking

● Bluetooth is a universal protocol for low power, near field 
communication operating at 2.4 - 2.485 GHz using spread spectrum

● The minimum specification for Bluetooth range is 10 meters

● When two Bluetooth devices connect, this is referred to as pairing. 

● Nearly any two Bluetooth devices can connect to each other. 

● Any discoverable Bluetooth device transmits the following 
information: 

    ○ Name

    ○ Class

    ○ List of services

    ○ Technical information
    Check…

● TO do A bluetooth Pentest u need a bluetooth 
adapter.

● Thank Goodness, our computer have it inside, 
and we can connect it to our Virtual machine 
too.

● Install the following

    sudo apt install bluetooth bluez bluez-tools 
    rfkill blueman

* Config…

● We will unblock our bluetooth 
device

● We will start the bluetooth service

● To get information about your 
bluetooth device.

    hciconfig 

● TO Scan the bluetooth nearby

    hcitool scan

# SS7 Attack

● An SS7 attack is a security exploit that takes advantage of a weakness in the 
design of SS7 (Signaling System 7) to enable data theft, eavesdropping, 
text interception and location tracking.

● To allow wireless cellular and wired connection, the SS7 phone signalling 
protocols are in charge of initiating and ending phone calls across a digital 
signalling network. Most international public phone calls are made over the Public 
Switched Telephone Network.

● Other apps were gradually incorporated into SS7. This made it possible to roll out 
new mass-market solutions, including call waiting, SMS, prepaid billing, number 
translation, call forwarding, local number portability, and conference calling.

● For this purpose u need a device that can intercept a cellular signals

# Reverse Engineering

● Reverse Engineering is one of the greatest Cyber Security 
Field.

● As the name suggests we will reverse any thing that is 
built up.

● Here Hackers will reverse engineer and Bypass many 
things, like the last time burp licencing.

● Every thing we use SOftwares are cracked by reverse 
engineers.

● For this You have to learn programming languages like, 
Assembly and C 

● There are many tools used to reverse any software and 
get the assembly code for further review.

○ Example: IDA, Ghidra, …

● And White hats, use this skill to reverse any malwares and 
to analyze it.
