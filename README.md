# Group_Project_Network

This network building exercise was completed as a group project by our team. We successfully presented our project to the class, providing an explanation of the steps we followed to set up the network.

Note: We utilized Cisco Packet Tracer for network simulation throughout the project.

## Components

For the local network:

-   1 router (Router 0)
-   1 switch for each department (Management, Secretariat, Study, Production)
-   4 sectors:
    -   Management: 5 posts
    -   Secretariat: 5 posts
    -   Study: 8 posts
    -   Production: 10 posts
-   2 support sectors (each with 30 posts)
-   1 DNS server
-   1 DHCP server
-   1 storage server (iSCSI)

Additional Components:

-   External server with IP 233.200.100.10
-   Router with IP 223.200.100.1/24 on port 0/0/1 and IP 192.170.1.2 on port 0/0/0
-   CloudPT, modem, and switch connected to Router 0 on port 0/0/1 with IP 192.170.1.1 to simulate internet access.

## Step-by-step Configuration

1.  **Configure Router 0:**
    
    
    
    -   We connected the company's end devices to Router 0's port 0/0/0 to establish internal connectivity.
    -   To do this, we assigned the IP address and subnet mask for port 0/0/0 as follows:
        -   IP: 192.168.100.254
        -   Subnet Mask: 255.255.255.0
    -   Next, we connected Router 0's port 0/0/1 to the external server, modem, and cloudPT to establish external connectivity.
    -   We configured port 0/0/1 with the following IP addresses:
        -   IP: 192.170.1.1
        -   Subnet Mask: 255.255.255.0
2.  **Configure DHCP server:**
    
    We enabled the DHCP server and connected it to the network.
    
    -   The DHCP server was set up to automatically assign DHCP IP addresses to end devices, using the default gateway 192.168.100.254.
3.  **Configure DNS server:**
    
    We connected the DNS server to the network.
    
    -   The DNS server was configured with an example address and assigned the IP 233.200.100.
4.  **Configure storage server:**
    
    We connected the storage server to the network.
    
    -   A static IP address was assigned to the storage server, such as 192.168.100.252, and the default gateway was set to 192.168.100.254.
    -   Additionally, we created an admin user account for secure access to the storage server.
5.  **Department setups:**
    
    Using Cisco Packet Tracer, we simulated the switches for each department (Management, Secretariat, Study, Production).
    
    -   The switches were connected to the network to establish communication between the departments.
    -   We segregated the departments by giving them their own switch witch also allows you to easily expand the network
6.  **External server and router setup:**
 
    -   The external server was connected to Router 0's port 0/0/1.
    -   We configured the external server with the IP 233.200.100.10.
    -   Router 0's port 0/0/1 was connected to the router with the IP 223.200.100.1/24 on port 0/0/1 and IP 192.170.1.2 on port 0/0/0.
    -   The modem and switch were connected to Router 0's port 0/0/1, with the switch being assigned the IP 192.170.1.1.

## Project Presentation

During the presentation to the class, our team explained the step-by-step configuration process and highlighted the key components of the network setup. We showcased the successful connections between the devices, including the routers, switches, servers, and end devices. The functionalities of the DHCP server, DNS server, and storage server were also demonstrated.

By working collaboratively and utilizing Cisco Packet Tracer for simulation, we successfully completed the network building exercise and presented our project with confidence to the class.
