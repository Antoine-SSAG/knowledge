Investigation sources:         # AbuseIPDB is a crowd-sourced collection of IPs associated with
        #   malicious activity
        
        AbuseIPDB: https://www.abuseipdb.com/check/$%7Bip%7D
        
        
        # AlienVault Open Threat Exchange provides IOCs and threat intel
        
        AlienVault: https://otx.alienvault.com/indicator/ip/$%7Bip%7D
       
       
        # apility.io aggregates multiple blacklists
        
        #apility.io: https://apility.io/search/$%7Bip%7D
        
        
        # ThreatCrowd presents AlienVault OTX's data in a different format
        
        ThreatCrowd: https://www.threatcrowd.org/ip.php?ip=$%7Bip%7D
        
        
        # Shodan records historical open ports and services on the host
        
        Shodan: https://shodan.io/host/$%7Bip%7D
        
        
        # Google searches the web for the IP
        
        Google: https://www.google.com/search?q=$%7Bip%7D
        
        
        # Google DNS uses Google's DNS over HTTPS service to do a PTR lookup on the IP
        
        Google DNS: https://dns.google.com/query?name=$%7Bip%7D
        
        
        # VirusTotal's passive DNS service displays historical DNS records for an IP
        
        VirusTotal: https://www.virustotal.com/gui/ip-address/$%7Bip%7D/relations
        
        
        # SecurityTrails's passive DNS service displays historical DNS records for an IP
        
        SecurityTrails: https://securitytrails.com/list/ip/$%7Bip%7D
        
        
        # Ipinfo requires a free account
        
        #Ipinfo: https://ipinfo.io/account/search?query=$%7Bip%7D
        
        
        # Auth0 Signals requires a free account
        
        #Auth0 Signals: https://auth0.com/signals/ip/$%7Bip%7D-report
        
        
        # Carbon Black provides additional endpoint data.
        
        #   Replace "YourCarbonBlackServer" with the IP or hostname of your
        #   Carbon Black server.
        #Carbon Black: https://yourcarbonblackserver/#/search/cb.urlver=1&cb.q.ipaddr=$%7Bip%7D&sort=start%20desc&rows=100&start=0
