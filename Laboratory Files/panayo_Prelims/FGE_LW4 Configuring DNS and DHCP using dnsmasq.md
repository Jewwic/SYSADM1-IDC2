+----------------------------------+------------------------+----------+
| ![](vertopal_                    |                        |          |
| e42cbf2a6f1141ac95e69c229b22ea87 |                        |          |
| /media/image1.png){width="2.4in" |                        |          |
| height="0.5881944444444445in"}   |                        |          |
|                                  |                        |          |
| SCHOOL OF INFORMATION AND        |                        |          |
| TECHNOLOGY                       |                        |          |
+----------------------------------+------------------------+----------+
| NAME:                            | DATE PERFORMED:        |  /75     |
+----------------------------------+------------------------+----------+
| Section:                         | DATE SUBMITTED:        |          |
+----------------------------------+------------------------+----------+

# SYSADM1 -- Configuring DNS and DHCP with dnsmasq

# Requirement: 

-   A virtual machine running Linux

    Tasks:

    1.  Install dnsmasq

        ![](vertopal_e42cbf2a6f1141ac95e69c229b22ea87/media/image2.png){width="2.46875in"
        height="0.84375in"}

    2.  Create a configuration file dns.conf

    3.  Add the following lines to the configuration file:

        interface=eth0 \# Replace with your network interface

        dhcp-range=192.168.1.100,192.168.1.200,24h

        domain=example.com \# Replace with your desired domain

        server=8.8.8.8 \# Specify a DNS resolver

    4.  Adjust the interface, dhcp-range, and domain values as needed
        > for your network.

    5.  Start dnsmasq

        ![](vertopal_e42cbf2a6f1141ac95e69c229b22ea87/media/image3.png){width="2.9166666666666665in"
        height="0.9166666666666666in"}

    6.  Connect a new device to the network and verify that it receives
        > and IP address from the DHCP scope

    7.  Configure a client devices to use the dnsmasq server as its DNS
        > resolver

    8.  Test connectivity by executing a two-way ping

    9.  Write a reflection about how Linux and Windows differ in terms
        > of setting DNS and DHCP.

        **Grading Rubric:**

  ----------------------------------------------------------------------------------
  **Criteria**      **Excellent     **Good (10)**  **Needs        **Unsatisfactory
                    (15)**                         Improvement    (0)**
                                                   (5)**          
  ----------------- --------------- -------------- -------------- ------------------
  DNS Configuration Successfully    Configures DNS Struggles to   Unable to
                    configures DNS  records but    configure DNS  configure DNS
                    records         may have minor records or has records or resolve
                                    errors or      significant    DNS queries.
                                    omissions.     errors.        

  DHCP              Correctly       Configures     Struggles to   Unable to
  Configuration     configures DHCP DHCP settings  configure DHCP configure DHCP
                    settings (lease but may have   settings or    settings or assign
                    time, IP        minor errors   has            IP addresses to
                    address range,  or omissions.  significant    clients.
                    etc.) and                      errors.        
                    assigns IP                                    
                    addresses to                                  
                    clients.                                      

  Connectivity      Successfully    Successfully   Struggles to   Unable to ping
                    pings devices   pings most     ping devices   devices within the
                    within the      devices but    within the     network or
                    network and     may have       network or     external hosts.
                    external hosts. occasional     external       
                                    connectivity   hosts.         
                                    issues.                       

  Troubleshooting   Effectively     Identifies and Struggles to   Unable to identify
                    identifies and  resolves most  identify or    or resolve issues.
                    resolves issues issues but may resolve        
                    related to DNS, require        issues.        
                    DHCP, or        assistance.                   
                    network                                       
                    connectivity.                                 

  Reflection        Offers          Provides some  Struggles to   No reflection
                    insightful and  reflections    articulate the provided.
                    thoughtful      but may lack   differences or 
                    reflections on  depth or       provides       
                    the differences clarity.       limited        
                    between setting                reflection.    
                    up DNS in Linux                               
                    and Windows.                                  
  ----------------------------------------------------------------------------------
