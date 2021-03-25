# advanced-leach
Advanced
Advanced Leach protocol proposed by doing following modifications to traditional leach protocol.

The Proposed Leach Protocol is similar to LEACH Protocol. It has two stages: setup phase and steady phase. The main difference occurs in the setup phase which leads to great  improvement in terms of lifetime of WSNs. In the setup phase of leach protocol, all the nodes select a random number from 0 to 1, then if the number is  less than or equal to threshold (T(N), as calculated previously) it becomes a cluster head (CH) else the node  remains ordinary. In advanced leach protocol along with threshold a new condition is introduced i.e the node energy should be greater than the average energy (Eavg).The process continues until all cluster heads are chosen. After all the  CHs are chosen, they broadcast advertisement messages to the overall network informing that it became a CH. 


Here comes another enhancement where a node must select a CH according to total distance  to reach the base station (i.e., distance from node to CH + distance from CH to BS), not a  CH that is closest to it. Distances are calculated according to the equation 1.11 and the  minimum of the total distance is chosen.
D (x, y) = √ (x1 - x2)2 + (y1 – y2)

After the ordinary node selects a cluster head that has the minimum distance, it sends a  message to inform a cluster head that it will be a member of its cluster. After a request 
message is received from ordinary nodes, the cluster heads make a time-division multiple  access (TDMA) schedule for each member in its cluster. The TDMA schedule assigns a  timescale for every ordinary member node in it; it means that every ordinary member node  is only allowed to send in its specific timescale, or else it has to wait (go in sleep mode).  After the setup stage is completed, a steady stage starts same as in the LEACH protocol.
