Netcat Clone
A lightweight Python implementation of the famous Netcat (nc) utility, designed for learning network programming, offensive security concepts, and client-server communication.

Features
TCP Client
TCP Server
Interactive Shell
Command Execution
File Transfer Support
Multi-threaded Connections
Custom Port Listening
Red Team / Pentesting Practice
Why This Project?

Netcat is often called the Swiss Army Knife of Networking because it allows security professionals to:

Open TCP connections
Transfer files
Create bind shells
Create reverse shells
Debug network services
Test firewall rules
Understand socket programming

This project was developed to better understand how these mechanisms work internally rather than relying on prebuilt tools.

Installation

Clone the repository:

git clone https://github.com/othmanemr-c/Netcat.git
cd Netcat

Run:

python3 netcat.py
Usage
Start a Listener
python3 netcat.py -l -p 4444
Connect to a Target
python3 netcat.py -t 192.168.1.10 -p 4444
Execute a Command
python3 netcat.py -l -p 4444 -e "whoami"
Upload a File
python3 netcat.py -t 192.168.1.10 -p 4444 < file.txt
Example

Listener:

python3 netcat.py -l -p 9001

Client:

python3 netcat.py -t 127.0.0.1 -p 9001
