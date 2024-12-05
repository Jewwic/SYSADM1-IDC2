![image](https://github.com/user-attachments/assets/93de4871-4639-4e57-8ce9-c1a059c4e421)


# SYSADM1 -- Capacity Management & Planning

## Part 1. A Simulated Dataset for Capacity Planning Exercise {#part-1.-a-simulated-dataset-for-capacity-planning-exercise .list-paragraph}

![](vertopal_90644493138445dc8ca6b8a687f7672a/media/image2.png){width="4.749564741907261in"
height="2.4791666666666665in"}**Scenario:** A mid-sized e-commerce
website is expecting a significant surge in traffic due to an upcoming
holiday sale.

### [Projected Traffic Increase]{.underline}

-   **Expected Peak Traffic:** 5x the normal peak traffic

-   **Peak Time:** 12:00 PM - 3:00 PM on the sale day

### [System Specifications]{.underline}

-   **Server Count:** 5

-   **CPU Cores per Server:** 8

-   **RAM per Server:** 32GB

-   **Network Bandwidth per Server:** 1Gbps

### [Additional Considerations]{.underline}

-   **New Product Launch:** A highly anticipated product will be
    released during the sale.

-   **Marketing Campaign:** A major marketing campaign will be launched
    to promote the sale.

-   **Potential Cyber Threats:** Increased traffic can attract malicious
    actors.

Tasks:

1.  Review the provided server performance data and identify potential
    bottlenecks

The server performance data indicates potential bottlenecks during the
anticipated traffic surge:

-   **CPU Utilization:** During normal operations, CPU usage reaches 60%
    at peak times. With traffic expected to increase fivefold, the CPU
    could become a bottleneck, potentially exceeding 100% capacity.

-   **Memory Utilization:** Memory usage at peak times is 70%. A
    significant increase in traffic might result in memory saturation,
    leading to system slowdowns or crashes.

-   **Network Bandwidth:** Current network utilization during peak hours
    is 200 Mbps (inbound) and 100 Mbps (outbound). As the volume of
    incoming traffic increases, the network may exceed the 1Gbps
    bandwidth limit allocated per server. This could lead to slower
    response times and potential service interruptions.

-   **Response Time:** At current peak levels, the response time rises
    to 300ms. A fivefold traffic increase Re eh in much slower response
    times, impacting user experience.

-   **Cybersecurity Threats:** Increased traffic may attract malicious
    actors, potentially leading to DDoS attacks or other cyber threats.

2.  Brainstorm possible solutions to address the identified bottlenecks.
    Propose potential solutions considering hardware and software-based
    solutions.

Here are possible solutions that we have come up with:

-   **Load Balancing:** Implement load balancing across multiple servers
    to distribute traffic evenly, preventing any single CPU from
    becoming a bottleneck.

-   **Increase CPU Capacity:** Consider upgrading to a more powerful CPU
    with higher clock speeds or additional cores to handle increased
    processing demands effectively.

-   **Memory Leak Detection:** Utilize profiling tools to identify and
    fix memory leaks in applications, which can lead to increased memory
    usage over time.

-   **Increase Bandwidth Allocation:** If possible, upgrade the network
    bandwidth allocation per server beyond 1Gbps to accommodate higher
    traffic loads without degradation in performance.

3.  Discuss the pros and cons of each proposed solution by filling out
    the table below.

+-------------+----------------+-----------+-------------+-----------+
| Proposed    |                | Cost      | Complexity  | Potential |
| Solution    |  ------------- |           |             | impact on |
|             |   Pros   Cons  |           |             | system    |
|             |                |           |             | pe        |
|             |  ------ ------ |           |             | rformance |
|             |                |           |             |           |
|             |                |           |             |           |
|             |  ------------- |           |             |           |
+=============+================+===========+=============+===========+
| Load        | Pros:          | ₱16,800   | Medium      | Si        |
| Balancing   |                | per month |             | gnificant |
|             | -              |           |             | im        |
|             |    Distributes |           |             | provement |
|             |     traffic    |           |             | in        |
|             |     evenly     |           |             | handling  |
|             |     across     |           |             | increased |
|             |     multiple   |           |             | traffic   |
|             |     servers    |           |             | and       |
|             |                |           |             | reducing  |
|             | -   Prevents   |           |             | latency   |
|             |     any single |           |             |           |
|             |     server     |           |             |           |
|             |     from       |           |             |           |
|             |     becoming   |           |             |           |
|             |                |           |             |           |
|             |    overwhelmed |           |             |           |
+-------------+----------------+-----------+-------------+-----------+
|             | Cons:          |           |             |           |
|             |                |           |             |           |
|             | -   Requires   |           |             |           |
|             |     additional |           |             |           |
|             |     hardware   |           |             |           |
|             |     or         |           |             |           |
|             |     software   |           |             |           |
|             |     setup      |           |             |           |
|             |                |           |             |           |
|             | -   Complexity |           |             |           |
|             |     in         |           |             |           |
|             |                |           |             |           |
|             |  configuration |           |             |           |
|             |     and        |           |             |           |
|             |     management |           |             |           |
+-------------+----------------+-----------+-------------+-----------+
| Increase    | Pros:          | ₱16,000   | Medium      | Major     |
| CPU         |                | to        |             | im        |
| Capacity    | -   Enhances   | ₱50,000   |             | provement |
|             |     processing |           |             | in        |
|             |     power for  |           |             | per       |
|             |     demanding  |           |             | formance, |
|             |                |           |             | e         |
|             |   applications |           |             | specially |
|             |                |           |             | under     |
|             | -   Can handle |           |             | heavy     |
|             |     more       |           |             | load      |
|             |     concurrent |           |             |           |
|             |     tasks      |           |             |           |
|             |                |           |             |           |
|             |    effectively |           |             |           |
|             |                |           |             |           |
|             | Cons:          |           |             |           |
|             |                |           |             |           |
|             | -   High cost  |           |             |           |
|             |     for        |           |             |           |
|             |     advanced   |           |             |           |
|             |     CPUs       |           |             |           |
|             |                |           |             |           |
|             | -              |           |             |           |
|             |  Compatibility |           |             |           |
|             |     issues     |           |             |           |
|             |     with       |           |             |           |
|             |     existing   |           |             |           |
|             |     hardware   |           |             |           |
|             |     may arise  |           |             |           |
+-------------+----------------+-----------+-------------+-----------+
| Memory Leak | Pros:          | ₱0 (open  | Medium      | Moderate  |
| Detection   |                | source    |             | im        |
|             | -   Identifies | tools) to |             | provement |
|             |     and        | several   |             | as leaks  |
|             |     resolves   | thousand  |             | are       |
|             |                | pesos for |             | fixed,    |
|             | inefficiencies | c         |             | leading   |
|             |     over time  | ommercial |             | to better |
|             |                | tools.    |             | memory    |
|             | -   Can lead   |           |             | m         |
|             |     to         |           |             | anagement |
|             |     long-term  |           |             |           |
|             |                |           |             |           |
|             |    performance |           |             |           |
|             |     gains by   |           |             |           |
|             |     freeing up |           |             |           |
|             |     memory     |           |             |           |
|             |     resources  |           |             |           |
|             |                |           |             |           |
|             | Cons:          |           |             |           |
|             |                |           |             |           |
|             | -   Requires   |           |             |           |
|             |     ongoing    |           |             |           |
|             |     monitoring |           |             |           |
|             |     and        |           |             |           |
|             |                |           |             |           |
|             |    maintenance |           |             |           |
|             |                |           |             |           |
|             | -   May not    |           |             |           |
|             |     provide    |           |             |           |
|             |     immediate  |           |             |           |
|             |     benefits   |           |             |           |
+-------------+----------------+-----------+-------------+-----------+
| Increased   | Pro:           | ₱28,000   | Low         | Major     |
| Bandwidth   |                | per month |             | im        |
| Allocation  | -   Directly   |           |             | provement |
|             |     addresses  |           |             | in        |
|             |     network    |           |             | network   |
|             |                |           |             | per       |
|             |    bottlenecks |           |             | formance, |
|             |                |           |             | reducing  |
|             | -   Improves   |           |             | latency   |
|             |     overall    |           |             | and       |
|             |     user       |           |             | enhancing |
|             |     experience |           |             | respo     |
|             |     during     |           |             | nsiveness |
|             |     peak times |           |             |           |
|             |                |           |             |           |
|             | Cons:          |           |             |           |
|             |                |           |             |           |
|             | -   Can be     |           |             |           |
|             |     expensive  |           |             |           |
|             |     depending  |           |             |           |
|             |     on service |           |             |           |
|             |     provider   |           |             |           |
|             |                |           |             |           |
|             | -   May        |           |             |           |
|             |     involve    |           |             |           |
|             |                |           |             |           |
|             |  renegotiating |           |             |           |
|             |     contracts  |           |             |           |
+-------------+----------------+-----------+-------------+-----------+

Grading Rubric:

  -------------------------------------------------------------------------------
  Criteria           Excellent \| 10pts Good \| 7pts        Needs Improvement \|
                                                            4pts
  ------------------ ------------------ ------------------- ---------------------
  **Problem          Accurately         Identifies the main Identifies a problem
  Identification**   identifies the     problem and         but lacks clarity or
                     primary problem    provides a basic    accuracy.
                     and provides a     explanation.        
                     detailed                               
                     explanation.                           

  **Solution         Proposes multiple  Proposes one or two Proposes a solution
  Proposal**         relevant solutions relevant solutions  but lacks feasibility
                     and provides       but lacks detailed  or relevance.
                     detailed           explanation.        
                     explanations,                          
                     including                              
                     potential                              
                     drawbacks and                          
                     benefits.                              

  **Evaluation of    Provides a         Provides a basic    Does not evaluate the
  Solutions**        thorough           evaluation of the   proposed solutions or
                     evaluation of the  proposed solutions, provides a
                     proposed           but lacks depth.    superficial
                     solutions,                             evaluation.
                     considering                            
                     factors like cost,                     
                     complexity, and                        
                     potential impact.                      

  Score:                                                    /30
  -------------------------------------------------------------------------------

**Part 2. Network Scalability Analysis**

Recall the e-commerce website scenario we discussed earlier. Given the
expected surge in traffic, analyze the provided network topology
diagram. Identify potential bottlenecks and areas where scalability
might be a concern. Propose specific strategies to improve the
network\'s scalability and performance to ensure a seamless user
experience during the peak traffic period. Consider factors such as
increased user demand, new applications, and security threats.

![](vertopal_90644493138445dc8ca6b8a687f7672a/media/image3.bin){width="5.049483814523184in"
height="3.8229166666666665in"}

**1. Single Uplink from Access Switches to Core Switch (Potential
Bottleneck)**

-   Each VLAN's layer 2 switch has a single uplink to the central core
    switch. This configuration might become a bottleneck, especially if
    the aggregated

-   Traffic from all servers exceeds the uplink capacity (1Gbps or
    higher, depending on the setup).

**3. Core Switch Load**

-   The core switch (likely a Layer 3 switch) will handle all traffic
    aggregation and routing. During peak traffic, it might face high
    processing loads, potentially leading to delays or dropped packets
    if not adequately provisioned.

**4. Lack of Redundancy**

-   The absence of redundant paths between switches and the server
    infrastructure means that a single point of failure (e.g., an uplink
    failure) could disrupt service.

**5. Potential Cybersecurity Risks**

-   The topology does not indicate any specific measures for handling
    DDoS attacks, unauthorized access, or other cyber threats, which
    could increase during the sale.

### 

### 

### 

### Is the Design Scalable and Redundant Enough?

-   **Scalability:** The addition of another edge router and core switch
    significantly enhances the network's scalability. With proper
    configuration, it can handle peak traffic effectively.

-   **Redundancy:** The redundant edge routers and core switches provide
    high availability, reducing the risk of single points of failure.

However, to ensure that the system remains efficient:

-   Evaluate bandwidth usage during peak times to avoid bottlenecks.

-   Plan for future growth by implementing modular and scalable
    hardware.

![](vertopal_90644493138445dc8ca6b8a687f7672a/media/image4.png){width="7.550387139107611in"
height="3.501725721784777in"}

**Improvements in the Latest Design**

1.  **Additional Edge Router**

    -   **Advantage:** Provides redundancy at the internet gateway. If
        one router fails, the second can take over, ensuring continuous
        connectivity.

    -   **Consideration:** Ensure proper routing protocols (e.g., BGP,
        HSRP, VRRP) are configured between the routers for failover and
        load balancing.

2.  **Additional Multilayer Switch**

    -   **Advantage:** Improves fault tolerance and scalability at the
        core layer. This also balances traffic from the edge and between
        access switches.

    -   **Consideration:** Implement redundancy protocols like Spanning
        Tree Protocol (STP) or Multi-Chassis Link Aggregation (MLAG) to
        avoid network loops and optimize failover time.

3.  **Redundant Links**

    -   The use of redundant uplinks between core switches, edge
        routers, and access switches ensures high availability and
        prevents single points of failure.

  ------------------------------------------------------------------------------
  Criteria          Excellent \| 10pts Good \| 7pts        Needs Improvement \|
                                                           4pts
  ----------------- ------------------ ------------------- ---------------------
  **Network         Accurately         Identifies key      Identifies some basic
  Analysis**        identifies         network components  network components
                    potential          and some potential  but lacks a
                    bottlenecks,       bottlenecks.        comprehensive
                    security risks,                        analysis.
                    and capacity                           
                    limitations.                           

  **Scalability     Proposes multiple  Proposes some       Proposes limited
  Planning**        relevant solutions relevant            scalability
                    and provides       scalability         strategies.
                    detailed           strategies but      
                    explanations,      lacks detail.       
                    including                              
                    potential                              
                    drawbacks and                          
                    benefits.                              

  **Evaluation of   Proposes           Provides a basic    Does not evaluate the
  Solutions**       comprehensive      evaluation of the   proposed solutions or
                    scalability        proposed solutions, provides a
                    strategies,        but lacks depth.    superficial
                    including specific                     evaluation.
                    recommendations                        
                    for hardware                           
                    upgrades, software                     
                    configurations,                        
                    and network                            
                    optimizations.                         

  **Proposed        Provides a         Provides a basic    Does not provide a
  Design**          detailed and       design but lacks    clear and detailed
                    well-justified     specific details    design.
                    design, including  and justifications. 
                    network diagrams,                      
                    configuration                          
                    details, and                           
                    implementation                         
                    plans.                                 

  **Evaluation and  Provides a         Provides a basic    Does not evaluate the
  Justification**   thorough           evaluation of the   proposed solutions or
                    evaluation of the  proposed solutions, provides a
                    proposed           but lacks depth.    superficial
                    solutions,                             evaluation
                    considering                            
                    factors like cost,                     
                    complexity, and                        
                    potential impact.                      

  Score:                                                   /50
  ------------------------------------------------------------------------------
