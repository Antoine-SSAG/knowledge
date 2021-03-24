# Links

Definition : 

What is should be :

- Proative
- Include evyrthin (IOT, Printer, Desktop, Network Gear)
- No assumptions : 
    - Analyze eveyrthing and check the businness reason 
    - Even if everything is working, check it 
- Review all the devices
3 possibilities : 
    - System is safe 
    - System is maybe compromised
    - I'm unsure so I need to analyse the logs 

- Start with the network 
    - See everything
    - Can't hide packet
    - Permit to check C2 communication 
    - Traffic from and to the internet 
    - Packet capture in Bro/Zeek 
    - Analyze in pair ( internal+external IP )
        Thing to see :
            1- Persistency of connexion (communication every X time)
            2- Abnormal protocol behavior ? 
            3- Check IP reputation 
            4- Check Internal IP information 
            5- Give a status : 
                - OK
                - Compromised
    - Put a score on the IP - From 0 to 100 
        - For each warning add X
        - Remove X for each normal comportment 
            - High Risk :
                - Persistency of Connexion
                - Unexpectected protocol on default protocol
    
    - K-Means --> Becoming useless beacause of Jittering, algorythm changing the beacon timing by X%
    -   use time buckets to check for beaconing even with Jitter
- Analyze DNS requests :
    - Top hitting DNS
    - List total FQDN per domain
        