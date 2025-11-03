# My Day1 Toolbox (examples)

- nmap -sC -sV -oA scans/target 10.10.10.10
- ffuf -u http://10.10.10.10/FUZZ -w /usr/share/wordlists/dirb/common.txt -mc 200,301 -o ffuf/day1_ffuf.json -of json
- curl -I http://10.10.10.10
- curl http://10.10.10.10/robots.txt
- subfinder -d example.com -o subfinder_output.txt
- sqlmap -u "http://10.10.10.10/vuln.php?id=1" --batch --dbs
- ./linpeas.sh | tee linpeas_output.txt
- git add . && git commit -m "day1: add initial commands.md" && git push
- ffuf -u http://10.10.10.10/FUZZ -w /usr/share/wordlists/raft-small-words.txt -mc 200 -o ffuf/results.txt
- curl -s "https://crt.sh/?q=%25.example.com&output=json" | jq '.[].name_value' | sort -u > crtsh_subs.txt
