<h1>Troubleshooting Static Routes</h1>

<h2>Description</h2>

PC1 and PC2 were unable to communicate due to misconfigurations on each router. To troubleshoot, commands like 'show ip int brief' and 'show ip route' were used in enable mode. On R1, the next-hop address was corrected to 192.168.12.2 for the 192.168.3.0 destination. On R2, the next-hop interface was set to g0/1 for traffic toward 192.168.3.0. On R3, interface g0/1's IP address was updated to 192.168.13.3 for proper connectivity. Once these corrections were made, PC1 and PC2 were able to successfully ping each other.

<h2>Languages and Utilities Used</h2>

- <b>Cisco Command Line Interface</b> 

<h2>Environments Used </h2>

- <b>Cisco Packet Tracer</b>

<h2>Program walk-through:</h2>

The IP address with the correct next-hop address was added to the routing table for the g0/0 interface. 
![Screenshot 2025-01-12 235126](https://github.com/user-attachments/assets/06a3f864-0985-4bb0-b7f1-90cf6ad81454)

In this case R1's next-hop address to reach the 192.168.3.0 destination can be seen via the static route denoted by 'S' in the routing table. 
![Screenshot 2025-01-17 225557](https://github.com/user-attachments/assets/1cae1d21-5f52-42ee-b34c-18dbdab6d4a9)

R2's next-hop interface was corrected to interface g0/1 for the 192.168.3.0 destination. 
![Screenshot 2025-01-17 231206](https://github.com/user-attachments/assets/3e567fd6-7003-49d7-9bb8-f1195c944d59)

R3's IP address for interface g0/0 was corrected to 192.168.13.3. 
![Screenshot 2025-01-17 232232](https://github.com/user-attachments/assets/ee0442f3-2d51-496b-9758-7954105365f3)

PC1 and PC2 are now able to ping eachother, meaning they can communicate over the network. 
![Screenshot 2025-01-17 225037](https://github.com/user-attachments/assets/92c6d97d-eaae-403d-a9e8-4ceb66977a55)

![Screenshot 2025-01-12 235513](https://github.com/user-attachments/assets/95004225-b6d5-4b26-a853-772a409c03cc)



