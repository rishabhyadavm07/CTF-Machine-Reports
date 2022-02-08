## Reduclously Easy

Rishabh Yadav | 08-02-2022

Admin console printed on the screen of the machine: 10.0.2.4:9090

Ran nmap scan on the target : 

Found :
```
Starting Nmap 7.92 ( https://nmap.org ) at 2022-02-08 06:33 EST
NSE: Loaded 155 scripts for scanning.
NSE: Script Pre-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
Initiating ARP Ping Scan at 06:33
Scanning 10.0.2.4 [1 port]
Completed ARP Ping Scan at 06:33, 0.04s elapsed (1 total hosts)
Initiating Parallel DNS resolution of 1 host. at 06:33
Completed Parallel DNS resolution of 1 host. at 06:33, 0.00s elapsed
DNS resolution of 1 IPs took 0.00s. Mode: Async [#: 1, OK: 0, NX: 1, DR: 0, SF: 0, TR: 1, CN: 0]
Initiating Connect Scan at 06:33
Scanning 10.0.2.4 [65535 ports]
Discovered open port 22/tcp on 10.0.2.4
Discovered open port 80/tcp on 10.0.2.4
Discovered open port 21/tcp on 10.0.2.4
Discovered open port 13337/tcp on 10.0.2.4
Discovered open port 22222/tcp on 10.0.2.4
Discovered open port 60000/tcp on 10.0.2.4
Discovered open port 9090/tcp on 10.0.2.4
Completed Connect Scan at 06:33, 1.68s elapsed (65535 total ports)
Initiating Service scan at 06:33
Scanning 7 services on 10.0.2.4
Completed Service scan at 06:33, 6.00s elapsed (7 services on 1 host)
Initiating OS detection (try #1) against 10.0.2.4
NSE: Script scanning 10.0.2.4.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 06:33
NSE: [ftp-bounce 10.0.2.4:21] PORT response: 500 Illegal PORT command.
Stats: 0:00:20 elapsed; 0 hosts completed (1 up), 1 undergoing Script Scan
NSE: Active NSE Script Threads: 1 (1 waiting)
NSE Timing: About 99.90% done; ETC: 06:33 (0:00:00 remaining)
Stats: 0:00:40 elapsed; 0 hosts completed (1 up), 1 undergoing Script Scan
NSE: Active NSE Script Threads: 1 (1 waiting)
NSE Timing: About 99.90% done; ETC: 06:33 (0:00:00 remaining)
Completed NSE at 06:33, 30.42s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.03s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
Nmap scan report for 10.0.2.4
Host is up, received arp-response (0.00053s latency).
Scanned at 2022-02-08 06:33:02 EST for 39s
Not shown: 65528 closed tcp ports (conn-refused)
PORT      STATE SERVICE    REASON  VERSION
21/tcp    open  ftp        syn-ack vsftpd 3.0.3
| ftp-anon: Anonymous FTP login allowed (FTP code 230)
| -rw-r--r--    1 0        0              42 Aug 22  2017 FLAG.txt
|_drwxr-xr-x    2 0        0               6 Feb 12  2017 pub
| ftp-syst: 
|   STAT: 
| FTP server status:
|      Connected to ::ffff:10.0.2.15
|      Logged in as ftp
|      TYPE: ASCII
|      No session bandwidth limit
|      Session timeout in seconds is 300
|      Control connection is plain text
|      Data connections will be plain text
|      At session startup, client count was 1
|      vsFTPd 3.0.3 - secure, fast, stable
|_End of status
22/tcp    open  ssh?       syn-ack
| fingerprint-strings: 
|   NULL: 
|_    Welcome to Ubuntu 14.04.5 LTS (GNU/Linux 4.4.0-31-generic x86_64)
|_ssh-hostkey: ERROR: Script execution failed (use -d to debug)
80/tcp    open  http       syn-ack Apache httpd 2.4.27 ((Fedora))
|_http-server-header: Apache/2.4.27 (Fedora)
| http-methods: 
|   Supported Methods: GET POST OPTIONS HEAD TRACE
|_  Potentially risky methods: TRACE
|_http-title: Morty's Website
9090/tcp  open  http       syn-ack Cockpit web service 161 or earlier
|_http-title: Did not follow redirect to https://10.0.2.4:9090/
| http-methods: 
|_  Supported Methods: GET HEAD
13337/tcp open  unknown    syn-ack
| fingerprint-strings: 
|   NULL: 
|_    FLAG:{TheyFoundMyBackDoorMorty}-10Points
22222/tcp open  ssh        syn-ack OpenSSH 7.5 (protocol 2.0)
| ssh-hostkey: 
|   2048 b4:11:56:7f:c0:36:96:7c:d0:99:dd:53:95:22:97:4f (RSA)
| ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDNvEvp4kqXX1H6FNqkKASBizY59uyLsqrLzLfT4R5vD8yuq+K0OqomxTiDwipMZTfQIRuBl2OzXX3rzRQ0aB+4EXyLbsxqNNP/+xRgPgFL6FPNI7j2rPGt+hQ6nmkpBJzzSpA4BBlGwvQt/i4LhrRoDsuD2JxQlmH1LNAlG6rE+xyqMTEgnfnO70pYzcmxDOixHiqTkbrsGnE6kIiyiOopwsR2E2KLPusFQJhEhsOOCJzurO7YYbDxQIwOMOox96SPtgti+4bnAVndLpo/IddtzZu3PB4SK43aIeGWgP7ONl6H0Cs1opW1EQSmdpww+Nu3fMlAlC+VMfmJNca8z9Np
|   256 20:67:ed:d9:39:88:f9:ed:0d:af:8c:8e:8a:45:6e:0e (ECDSA)
| ecdsa-sha2-nistp256 AAAAE2VjZHNhLXNoYTItbmlzdHAyNTYAAAAIbmlzdHAyNTYAAABBBKqM0Vcrgqds3NsV5wJ7j876UEKSpMytY6gNpa0Ey47sSAizc+hUU8UGoFmPsco2rjIn9QhdEIWzeMJksnpbxDk=
|   256 a6:84:fa:0f:df:e0:dc:e2:9a:2d:e7:13:3c:e7:50:a9 (ED25519)
|_ssh-ed25519 AAAAC3NzaC1lZDI1NTE5AAAAIHJ5AJGj4+y9xHabmQ5cLyxySqPvQ9sW+ko0w1vnzZWI
60000/tcp open  tcpwrapped syn-ack
|_drda-info: ERROR
2 services unrecognized despite returning data. If you know the service/version, please submit the following fingerprints at https://nmap.org/cgi-bin/submit.cgi?new-service :
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port22-TCP:V=7.92%I=7%D=2/8%Time=620254F0%P=x86_64-pc-linux-gnu%r(NULL,
SF:42,"Welcome\x20to\x20Ubuntu\x2014\.04\.5\x20LTS\x20\(GNU/Linux\x204\.4\
SF:.0-31-generic\x20x86_64\)\n");
==============NEXT SERVICE FINGERPRINT (SUBMIT INDIVIDUALLY)==============
SF-Port13337-TCP:V=7.92%I=7%D=2/8%Time=620254F0%P=x86_64-pc-linux-gnu%r(NU
SF:LL,29,"FLAG:{TheyFoundMyBackDoorMorty}-10Points\n");
MAC Address: 08:00:27:BF:52:95 (Oracle VirtualBox virtual NIC)
Device type: general purpose
Running: Linux 3.X|4.X
OS CPE: cpe:/o:linux:linux_kernel:3 cpe:/o:linux:linux_kernel:4
OS details: Linux 3.2 - 4.9
TCP/IP fingerprint:
OS:SCAN(V=7.92%E=4%D=2/8%OT=21%CT=1%CU=32475%PV=Y%DS=1%DC=D%G=Y%M=080027%TM
OS:=62025515%P=x86_64-pc-linux-gnu)SEQ(SP=103%GCD=1%ISR=10D%TI=Z%CI=I%II=I%
OS:TS=A)OPS(O1=M5B4ST11NW7%O2=M5B4ST11NW7%O3=M5B4NNT11NW7%O4=M5B4ST11NW7%O5
OS:=M5B4ST11NW7%O6=M5B4ST11)WIN(W1=7120%W2=7120%W3=7120%W4=7120%W5=7120%W6=
OS:7120)ECN(R=Y%DF=Y%T=40%W=7210%O=M5B4NNSNW7%CC=Y%Q=)T1(R=Y%DF=Y%T=40%S=O%
OS:A=S+%F=AS%RD=0%Q=)T2(R=N)T3(R=N)T4(R=Y%DF=Y%T=40%W=0%S=A%A=Z%F=R%O=%RD=0
OS:%Q=)T5(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)T6(R=Y%DF=Y%T=40%W=0%S
OS:=A%A=Z%F=R%O=%RD=0%Q=)T7(R=Y%DF=Y%T=40%W=0%S=Z%A=S+%F=AR%O=%RD=0%Q=)U1(R
OS:=Y%DF=N%T=40%IPL=164%UN=0%RIPL=G%RID=G%RIPCK=G%RUCK=G%RUD=G)IE(R=Y%DFI=N
OS:%T=40%CD=S)

Uptime guess: 20.810 days (since Tue Jan 18 11:07:48 2022)
Network Distance: 1 hop
TCP Sequence Prediction: Difficulty=259 (Good luck!)
IP ID Sequence Generation: All zeros
Service Info: OSs: Unix, Linux; CPE: cpe:/o:linux:linux_kernel

TRACEROUTE
HOP RTT     ADDRESS
1   0.53 ms 10.0.2.4

NSE: Script Post-scanning.
NSE: Starting runlevel 1 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
NSE: Starting runlevel 2 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
NSE: Starting runlevel 3 (of 3) scan.
Initiating NSE at 06:33
Completed NSE at 06:33, 0.00s elapsed
Read data files from: /usr/bin/../share/nmap
OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 40.33 seconds
           Raw packets sent: 23 (1.806KB) | Rcvd: 15 (1.278KB)
```


Visited port with 9090 and found a flag: 
`FLAG {There is no Zeus, in your face!}` - 10 Points

Nmap scan showed that ftp allows anonymous login 
signed in and found 2 files named flag and pub directory
`get FLAG.txt`
`FLAG{Whoa this is unexpected}` - 10 Points

while reading the nmap scan report found out a port 13337 which is providing a flag : 
`FLAG:{TheyFoundMyBackDoorMorty}`-10Points





