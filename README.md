# Disgruntled

## Objective
Perform a Linux forensic investigation on a compromised system used by a disgruntled insider. The objective was to identify malicious commands executed, files accessed or exfiltrated, and reconstruct the attacker's timeline using system artifacts.

### Skills Learned
- Linux command history and bash artifact analysis
- Log analysis (auth.log, syslog, cron)
- Insider threat investigation methodology
- Timeline reconstruction from system artifacts
- File integrity and access tracking

### Tools Used
- Linux CLI (bash, cat, grep, find, last, who)
- Auth.log and syslog analysis
- Bash history file examination
- File metadata inspection (stat, ls -la)

## Steps
Investigation began by reviewing the .bash_history file to identify commands executed by the suspect user. Auth.log was analyzed to correlate login times and privilege escalation attempts. Cron jobs were inspected for persistence mechanisms. File access times were cross-referenced against the suspect's known working hours to identify anomalous activity. A full timeline was constructed documenting every malicious action from initial access to data staging.

*Ref 1: .bash_history showing sequence of suspicious commands*
![p1](https://github.com/user-attachments/assets/00adef31-d3b4-477b-8349-bda6405c736e)

![P2](https://github.com/user-attachments/assets/214a99d5-3426-48b9-b646-a0efbb6aea6e)
*Ref 2: Auth.log entries confirming unauthorized sudo usage*
![P3](https://github.com/user-attachments/assets/12da8adf-1d63-4685-bd1c-ef08dfb8fc48)

![P4](https://github.com/user-attachments/assets/12927c41-8007-4f31-b081-543a07bb3da9)

![P5](https://github.com/user-attachments/assets/f6083b85-f423-41b3-b980-961f8f5f4753)

![P6](https://github.com/user-attachments/assets/969f99f7-7cfa-4747-825a-adc86ddda75a)

![P7 past](https://github.com/user-attachments/assets/bedf982c-3e5e-4c66-a9b4-60ecec05fea0)

![P7 past 2](https://github.com/user-attachments/assets/6b4a1415-bbb4-4f92-9e2b-a77686e1f0a6)

![P7](https://github.com/user-attachments/assets/71ec757c-86f1-4926-affe-0be87a64d53c)






