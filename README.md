# University-Network-Management-System
This project simulates a complete university network infrastructure using Cisco Packet Tracer. It demonstrates how to design, configure, and manage a multi-departmental network, including wired and wireless connectivity, DHCP configuration, routing, and internet access.

Network Architecture
    Admin Block: Central router and switch managing the entire university network, connected to ISP for internet access. Hosts the main DHCP server for some departments.
    Departments: Separate routers and switches for each department (SET, Arts, Exam), connected to Admin Router. Each department has labs (wired PCs), classrooms and staff rooms (wireless enabled).
    Hostels: Separate subnet managed by Hostel Router, with switches and wireless routers providing Wi-Fi for boys and girls hostels.
    Internet Access: Provided through an ISP router connected to Admin Router.

Devices Used
    Cisco Routers (2811, 1941, etc.)
    Cisco Switches (2960)
    Wireless Routers (WRT300N) as access points
    PCs and Laptops as clients
    ISP Router (simulated)

Key Features
    Segmented departmental networks with individual DHCP pools.
    Centralized internet access via Admin Router.
    Wireless access points for staff rooms and classrooms.
    Wired connections for labs for enhanced reliability.
    Separate subnets for hostels with DHCP managed by Hostel Router.
    Routing and static routes configured for inter-departmental communication.

IP Addressing Scheme
Department	Subnet	Default Gateway
Admin & Exam	192.168.10.0/24	192.168.10.1
SET	192.168.20.0/24	192.168.20.1
Arts	192.168.30.0/24	192.168.30.1
Hostel Boys	192.168.50.0/24	192.168.50.1
Hostel Girls	192.168.51.0/24	192.168.51.1

How to Use
    Open the Packet Tracer file located in the Topology folder.
    Explore the network devices and connections.
    Review router and switch configurations in the Configs folder.
    Use the console to test connectivity, DHCP assignment, and routing.
    Modify or extend the topology as per your requirements.

Challenges Faced
    Configuring DHCP across multiple subnets and disabling DHCP on wireless routers.
    Managing IP addressing to avoid overlaps and conflicts.
    Ensuring connectivity between multiple routers and switches.
    Setting up wireless access points correctly as bridge devices.

Future Enhancements
    Add firewall for network security.
    Implement VLANs for better traffic segmentation.
    Introduce network monitoring tools.
    Integrate authentication servers for user management.

Author
Karthikeyan T
