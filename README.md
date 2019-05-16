DNS:
  Host (A: ipv4, AAAA: ipv6)
      E.g.: 
      Type: A
      Name: @
      Value: Parked
  Alias (CNAME)
  
      E.g.: 
      Type: CNAME
      Name: www
      Value: @
  Mail Exchanger (MX)
      Can have multiple MX as multiple mail servers. Mail delivery will try by using priority.
      
  Service Record (SRV)
      Contain data about the service. Usually created automatically by applications
      - Service (E.g. LDAP)
      - Target (Host that offers that service)
      - Port
      - Priotiry (Lower is preferred)
      
  Start of Authority (SOA)
      - One per zone
      - Primary name server
      - E-mail of administrator
      - Serial number
      - Refresh time for the zone
      
  Name Server (NS)
    - Contains authority DNS Servers for that domain
    - Can be DNS server with secondary zones
    - Is the best source to answer queries
    
  Pointer (PTR)
    - Provide IP Address to Name mapping
    - Opposite of A or AAAA records
    - Ued for reverse lookup tools
    - Not required to run Active Directory
  
 Godaddy DNS defaut setting 
Records

Type	Name	Value	TTL	Actions
A	@	Parked	600 seconds	Edit
CNAME	www	@	1 Hour	Edit
CNAME	_domainconnect	_domainconnect.gd.domaincontrol.com	1 Hour	Edit
NS	@	ns15.domaincontrol.com	1 Hour	
NS	@	ns16.domaincontrol.com	1 Hour	
SOA	@	Primary nameserver: ns15.domaincontrol.com.	1 Hour	
