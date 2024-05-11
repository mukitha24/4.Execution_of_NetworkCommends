# 4.Execution_of_NetworkCommands
## AIM :Use of Network commands in Real Time environment
## Software : Command Prompt And Network Protocol Analyzer
## Procedure: To do this EXPERIMENT- follows these steps:
In this EXPERIMENT- students have to understand basic networking commands e.g cpdump, netstat, ifconfig, nslookup ,traceroute and also Capture ping and traceroute PDUs using a network protocol analyzer
All commands related to Network configuration which includes how to switch to privilege mode
and normal mode and how to configure router interface and how to save this configuration to
flash memory or permanent memory.
This commands includes
• Configuring the Router commands
• General Commands to configure network
• Privileged Mode commands of a router
• Router Processes & Statistics
• IP Commands
• Other IP Commands e.g. show ip route etc.
## CODE
## SERVER
```
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    ip=input("Enter the website you want to ping ") 
    s.send(ip.encode()) 
    print(s.recv(1024).decode())
```
## TRACEROUTE COMMAND
```
from scapy.all import* 
target = ["www.google.com"] 
result, unans = traceroute(target,maxttl=32) 
print(result,unans)
```
## SERVER
```
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    ip=input("Enter the website you want to ping ") 
    s.send(ip.encode()) 
    print(s.recv(1024).decode())
```
## Output
## PING COMMAND
## CLIENT
![image](https://github.com/mukitha24/4.Execution_of_NetworkCommends/assets/154068225/b8ca5e7f-0e7e-45bc-8c5c-3152b1a08540)
## SERVER
![image](https://github.com/mukitha24/4.Execution_of_NetworkCommends/assets/154068225/71f7614e-e86d-46e3-8bbf-d3343195134e)
## TRACEROUTE COMMAND
![image](https://github.com/mukitha24/4.Execution_of_NetworkCommends/assets/154068225/58edc849-3835-4558-a493-773dae78871c)

## Result
Thus Execution of Network commands Performed 
