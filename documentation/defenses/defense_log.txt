### Technical Observation: Network State
- **Finding:** \`network_state.txt\` appeared blank during initial capture.
- **Analysis:** This is expected behavior for a high-speed brute force attack. The TCP sessions are opened and closed so rapidly that manual 'snapshot' commands (ss/netstat) may miss the active window. 
- **Remediation:** Forensic analysis should pivot to persistent system logs (/var/log/auth.log) for reliable evidence.
