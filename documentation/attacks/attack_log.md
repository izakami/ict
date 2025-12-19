update: Manual service Enablement
-observation: INitial reconnaissance showed all ports were closed(Hardened state).
Action taken: Manually enabled SSH (port22) on the target.
reason: in a production environment,s ervices like ssh must remain open for administration. We enabled this to simulatea realistic attack surface for testing.
 hydra brute force result
Wordlist: fasttrack.txt
result: no valid password found. THis indicates the user likeing is using common password.
