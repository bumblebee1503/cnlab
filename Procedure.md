A simplified procedure to create a LAN and WAN connection using two switches and two routers in Cisco Packet Tracer:

Setting Up the LAN and WAN:

1. Open Cisco Packet Tracer:
   - Launch Cisco Packet Tracer on your computer.

2. Add Devices:
   - Drag and drop the following devices from the left panel to the workspace:
     - 2 Routers
     - 2 Switches
     - 20 PCs (10 PCs for each LAN)

3. Connect Devices within Each LAN:
   - Connect PCs to Switches:
     - Use the Connections tool (lightning bolt icon).
     - Click on a PC, select FastEthernet0, and then click on the switch and select an available port. Repeat this for the second PC and switch.
   - Connect Switches to Routers:
     - Connect each switch to its respective router:
       - Click on the switch, select FastEthernet0/1 (or any other available port), then click on the router and select GigabitEthernet0/0 (or another available port).

4. Connect the Routers to Form a WAN:
   - Use a Serial or Ethernet cable to connect the two routers:
     - Click on one router, select Serial0/0/0 (or GigabitEthernet0/1 if using Ethernet), and then click on the other router and select the corresponding port.

5. Assign IP Addresses:
   - On the PCs:
     - Click on each PC, go to the Desktop tab, then click on IP Configuration.
     - Assign IP addresses within the same range for each LAN (e.g., 192.0.0.1 for the first PC, 192.0.0.2 for the second, with a subnet mask of 255.255.255.0).
   - On the Routers:
     - Double-click each router, go to the Config tab, and set IP addresses for the interfaces connected to the switches (e.g., 192.0.0.254 for the first router’s LAN interface) and the interface connecting to the other router (e.g., 192.0.0.1 and 192.0.0.2 for the serial interfaces connecting the routers).

6. Enable Routing Between LANs:
   - Go to each router's Config tab, find the Routing section, and add the connected networks to allow communication between the two LANs.

7. Test the Connectivity:
   - Use the Command Prompt on one PC to ping a PC in the other LAN to ensure they can communicate across the WAN.

This setup uses two routers and two switches to connect two LANs and form a WAN, allowing you to simulate both local and wide area network communication.
