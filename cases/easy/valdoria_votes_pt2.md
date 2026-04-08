## Valdoria Votes: A Political Mystery

A hacking group claims to have hacked into the voting poll machines that people were meant to utilize. The ip used to do this was 55.49.227.170. They forgot to take this off from a poster they posted bragging they hacked them. 


#### General 

- The ip 55.49.227.170, resolves to two domains including "valdoriavotesgov.com" and "shadow-hackers-r.us". 

    - in particular, the fake government site resolves to 3 ips, 55.49.227.170, 214.85.104.248, and 157.100.244.104

- The legitimate website for the Valdoria Elections Board is "valdoriavotes.gov"

- While they were doing reconnaissance, they are specifically interested in "new hires", the prevention measure they are interested in is "election interference", the machines they are targeting are voting machines, and they were trying to get its "technical manual". 


#### Suspicious  

Anderson Snooper clicked on a phishing email and entered his username and password into the "valdoriavotesgov.com" website with no MFA enabled. 

- ip: 10.10.0.4
- username: ansnooper 
- email: anderson_snooper@valdoriavotes.gov

Now that the threat actor has gained access to his email, he ask Barry Schmelly on ways to access it since he is the boss of Anderson. 

The threat actor seems to use chatGPT to ask about the Election Commissioner. 

- ELection Commissioner: Array Bobama 
- ip: 10.10.0.13
- email: arrack_bobama@valdoriavotes.gov
- hostname: QDPG-DESKTOP
- MFA: False

The threat actor was able to reset the password and log into his account. This happened at 2024-10-16T00:00:00.000Z, and the ip address used was 214.85.104.248