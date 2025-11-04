# Linux CloudOps Commands Cheat Sheet
## Networking
| Command | Purpose | Example |
|---------|---------|---------|
|`nc HOST PORT` | Connect to TCP port | `nc localhost 30000` |
| `nmap -sV -p RANGE HOST` | Scan ports + services | `nmap -sV -p 31000-32000 localhost` |
| `openssl s_client` | Test SSL/TLS | `openssl s_client -connect localhost:443` |

## File Operations
| Command | Purpose | Example |
|---------|---------|---------|
| `diff file1 file2` | Compare files | `diff passwords.new passwords.old` |
| `xxd -r` | Reverse hexdump | `xxd -r data.txt > binary` |

## Text Processing
| Command | Purpose | Example |
|---------|---------|---------|
| `grep PATTERN file` | Search text | `grep ERROR /var/log/messages` |
| `awk` | Process columns | `ps aux \| awk '{print $1, $11}'` |


