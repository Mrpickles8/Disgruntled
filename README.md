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
*Ref 2: Auth.log entries confirming unauthorized sudo usage*
