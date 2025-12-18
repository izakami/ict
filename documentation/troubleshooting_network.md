Network and auth troubleshooting log
issue 1: static ip and internet loss
symptom: after setting a static ip (192.168.4.20), the internt stopped working
root cause: DNS and Gateway were not properly configured in the manual setting
solution: reconfigured the connection using "nmcli" to include fateway (192.168.4.1) and google DNS (8.8.8.8)

issue 2 : Github Authentication failure
symptom: "git push" failed due to the 2021 password deprecation
attempt 1: tried personal access token (HTTPS)
attempt 2: cahnged to SSH keys for better security
Root cause of failure: Manul file name "pulic" caused pathing errors and libcrypto corruption
final solution: performed a clean slate reset. deleted "~/.ssh", regenerated a standard "id_ed25519" key and linked ther public key to github.
