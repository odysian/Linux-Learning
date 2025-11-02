# Linux-Learning
### Bash Scripting
Find files in cd with .log that have been modified in past 24hrs:  
`find . -name "*.log" -mtime -1` 

Created script in vim to [analyse-logs](Logs/analyse-logs.sh)
```sh
find . -name "*.log" -mtime -1

grep "ERROR" application.log
grep -c "ERROR" application.log
grep -c "FATAL" application.log

grep -c "FATAL" system.log
grep -c "CRITICAL" system.log
grep "CRITICAL" system.log
```

Give execute perms:  
`chmod +x analyse.logs.sh`

Run script:  
`./analyse-logs.sh`