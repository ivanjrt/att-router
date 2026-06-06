I'm making this repo cause I switched to AT&T not by choice by the way I'm forced because no other ISP is available in my area.
coming from Cable ISP, they claim it is faster, which on paper it is, but I don't feel that much of a difference, the upload speed is a bit faster, -no deny there.
therefore since there are a lot of things to remember, I'm writing this cheat sheet. 
ps. Yes I'm also a network Engineer, and I found their GUI from the early 2000s


Things that I know so far:
- Its IP address is pointing to `192.168.1.254`, why?
  
- It's DHCP starts delivering IPs past the `192.168.1.1-10` -why?, unless you manually change this
  
- The router needs to be restarted every noun then, even when it was just working few minutes ago.

- There's an app that connects to your phone and tells you when a device has been connected to the network, that is really good
  However, it also `scans` your devices for vulnerabilities, then it throws false positives and doesn't really give you any description on what found wrong - This is very annoying 
  
- not only that, but sometimes all your devices will lose wifi even though is back online, you need to turn on/off your wifi slider on your device

- There's no way in the router to add your own custom `DNS` apparently, this is their thing to watch customers, unless of course, you bypass your DHCP or manually change your devices to point to it.

- To open Ports, they only make available what they think one is going to use, but not docs on how to do your own.
1. Step 1: find your device from the list that you want to open the ports for, get its name/ip -this is crucial
   <img width="1264" height="232" alt="image" src="https://github.com/user-attachments/assets/fa416a8e-994f-4f4b-b080-13767b2e8924" />
Note: if your device has several NICs then this router will only register one, so as long you get one, is not problem

2. Go go `NAT/Gaming`
<img width="1662" height="234" alt="image" src="https://github.com/user-attachments/assets/642a4095-6060-4f6b-aafd-526ca5944916" />

3. Because most likely your custom port `wireguard` will not be on the list, then select `custom services`
   
<img width="558" height="145" alt="image" src="https://github.com/user-attachments/assets/89d415d9-a514-4360-9fb0-ba94e94cc6ec" />

then add the WireGuard usual port*:

<img width="933" height="539" alt="image" src="https://github.com/user-attachments/assets/265c72a2-11eb-473e-9adf-3d5f801b3d0c" />

Then select your device in question against the service (I've done `pcanywhere` for context)

<img width="1275" height="351" alt="image" src="https://github.com/user-attachments/assets/be4fabce-f40b-4298-80a6-35735873eb69" />
  
