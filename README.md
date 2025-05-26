**#Elevate Lab Task-1**
i have scaned my ip address for the open ports and analyzed the result.

**#Result**
PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
8090/tcp open  opsmessaging

**#Common Services running on the port and potential security for these ports**
PORT   Protocol   Service           Description                                                       Security Risk
135     TCP        msrpc            Microsoft RPC (Remote Procedure Call)                             Can be exploited by malware (e.g., Blaster worm)
139     TCP        netbios-ssn      NetBIOS Session Service (Windows File/Printer sharing)            Exposes file sharing to the network
445     TCP        microsoft-ds     SMB (Server Message Block) over TCP                               Exposes file/printer sharing to attackers
8090    TCP        opsmessaging     Often used by applications (e.g., Apache Tomcat, custom apps)     May expose web admin panels or APIs
