The EthernetCanGateway_tester configuration is a simulation that demonstrates how to implement a bidirectional CAN/Ethernet gateway using IpV4.

For the Ethernet to CAN transmission:
The Gateway (client) shall first receive a UDP-Frame to start. This frame can be sent by the Ethernet IG (server).
It contains two CAN frames to be sent. Each CAN frames is defined with at least 14 bytes for the CAN-Id, -dlc, -rtr and the data bytes. 

For the CAN to Ethernet transmission:
The CAN frames to be sent on Ethernet are simulated with an I-Generator. The Ethernet multi cast communication is based on a UDP socket managed by the Windows TCP/IP stack and the port 23. 