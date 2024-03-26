<img width="730" alt="Screenshot 2024-03-26 at 12 54 43 PM" src="https://github.com/learningdebunked/NetworkFundamentals/assets/7702406/c389865c-8d20-419d-a2b8-08511fae07c3">
# NetworkFundamentals

** DNS **

** GSLB **

** MAC Address ( media access controls - 48 bits , 1st 24 bits of vendor code)  is a physical address. Is coded by manufacturer and is a burn in address **

** IPV4 - logical address -  addressed to be assigned to the device , 32 bits in length , 8 bit groups  ( called the octet ). We have run out **

** NAT( Network address translation )** -- we have run out of IPV4 **

** IPV6 ** -- made of 128 bits ** -- written using hexadecimal , group of 4 called quartet , has 8 of quartets in all 

** NIC ( network interface card ) - 2 types - internal and external **

** Ethernet switch & flooding ** //TODO more 

** router & ip routing table  ** routing protocol (ospf) ** Connects two n/w of  switches

    ** internet routing table is about 800K routes ***
    ** route with longest bits in the subnet mask **
    ** switches makes forwarding decisions based on  mac addresses **
    ** Routers makes forwarding decisions based on ip addresses **
    ** Wireless access points or APs {access points}  & roaming **


** twisted pair cabling ** twisted to avoid electro magnetic interference
   
    ** unshielded twisted pair **
    ** shielded twisted pair **
    ** Plenum cable and RJ45 connectors ** T568B coding , which pin goes where ??
    ** Category of twisted cable means the bandwidth we support ** //TODO

** Fiber optic cable **
   
   ** SMF (  smaller diameter when compared to MMF) , typically used for long distance applications because it doesn't suffer from delayed distortion
   ** MMF ( diameter is larger )

           ** Mult0mide delay distortion

** NIC VS Accesspoint VS Switch Vs Router //TODO

** OSI Model ( Open systems interconnection ) ( Way to remember: **A**ll **P**eople **S**eem **T**o **N**eed  **D**ata **P**rocessing ) 

         ** **B(Bits)**eacon **F(frames)**rying **P(packets)**roduces **S(segments)**alvation
         ** OSI is just a reference model 

** TCP Model ( There can be 4 Layered or 5 layered model ) 

** TCP VS UDP ( when to use what and how is this used by SWE applications like Zoom or others ? )

    ** TCP - Reliable communication , transmission is succesful
    ** UDP - UnReliable communication
    ** The Data Link layer (i.e. Layer 2) is concerned with physical addressing. 
        For example, an Ethernet switch learns Layer 2 MAC addresses. Therefore, an Ethernet switch is considered to be a Data Link layer device.
    ** Obtaining IP address information from a server through an exchange of Discover, Offer, Request, 
       and Acknowledgement messages is a function of Dynamic Host Configuration Protocol (DHCP). DHCP uses UDP port 67.

** TCP and UDP reside at the Transport Layer of the OSI Model, which is also known as Layer 4. 
** Protocols at the application layer **

    ** HTTP - uses TCP Port 80
    ** HTTPS - Secure and uses TCP Port 443
    ** DNS - DNS Protocol , can use TCP or UDP Port 53 
    ** NTP ( Network Time Protocol ) - Is used to learn about time from external sources ( uses UDP port 123 )
    
    ** DHCP ( Dynamic host configuration protocol )  - Automatically assign IP Addresses ( uses UDP Port 67 ) 
    
           ** DHCP Server that can hand out IP Address to all of network devices 
           ** DHCP IPV4 vs DHCP IPV6 ( stateful vs stateless ) 

                        ** Neighbor discover Protocol ( NDP )
                        ** EUI 
           ** DORA ( Discover Offer Request Acknowledgment ) 
           
           <img width="909" alt="Screenshot 2024-03-25 at 8 41 43 AM" src="https://github.com/learningdebunked/NetworkFundamentals/assets/7702406/c8246e27-6839-4d4e-b18e-560975314c76">

           - In the offer stage , DHCP sends the IP address ofthe DHCP server 
           - After this the client requests this corresponding Server for a IP 
           - DHCP acknowledges the client with IP Address /Subnet mask and gateway
           -- DHCP Relay agent //TODO , when there is a router in the middle we have to do this
           --Stateful DHCP V6 vs Stateless DHCP V6 Servers
           -- Stateful ( prefix /length , host and dns server's ipv6 address )
           - stateless ( prefix length {gets n/w info from router} ) through NDP ( n/w discover protocol  , using a process call EUI-64)

           -- TODO EUI & NDP


           ** DNS OVERVIEW **
           
<img width="716" alt="Screenshot 2024-03-26 at 12 53 44 PM" src="https://github.com/learningdebunked/NetworkFundamentals/assets/7702406/8996a978-267d-41b4-bbed-37f8a8770203">

<img width="730" alt="Screenshot 2024-03-26 at 12 54 50 PM" src="https://github.com/learningdebunked/NetworkFundamentals/assets/7702406/9ffdfe2f-72c2-49a0-b582-b6e1d2d57ba4">

           - routers route based on IP Address and not on DNS Names
           - Domain name system
           

    
    
