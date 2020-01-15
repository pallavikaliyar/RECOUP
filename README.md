This is the readme for proof of concept implementation for SERI or RECOUP (A Robust Multicast Communication Protocol for Low Power and Lossy Networks)

The code presented in this project maybe ported for implementations which provides multicast engine. 

Section I : General Instructions and Notes -------->

1. Copy the contiki folder in your home directory of contiki-OS.
2. The paths for core, net, ip6 etc.are arranged exactly Contiki 3.x
3. While modifying the make file, please use Sublime or vim. Other editors might give trouble with whitespace.
4. All code/implementations can be found in the directory RECOUP/home/user/contiki/core/
5. For all the implementations, SERI Multicast engine has been used. By default ROLL engine is used , this should be modified for use cases where root is the only multicast sender i.e a P2MP scenario with root as sender. 
For changing the multicast engine in project-conf.h file of the project change the engine , for example 

Please set #define UIP_MCAST6_CONF_ENGINE UIP_MCAST6_ENGINE_SERI engine to multicast to use the code.

6. The rpl objective has been modified in the rpl_of0 file itself which is found in /home/user/contiki/core/net/rpl folder .


7. The code for the SERI multicast engine can be found on the path RECOUP/core/net/ipv6/multicast/ with the file names seri.c and seri.h

8. In order to see the arrows between the nodes upon receiving the packets i.e when a node receives the packet from its parents , 
#define DEBUG DEBUG_ANNOTATE should be set and ANNOTATE("#L %u 1\n", parent_ipaddr->u8[sizeof(uip_ipaddr_t) - 1]); should be added to 
/home/user/contiki/core/net/ipv6/multicast/seri.c file . If the arrows are not required set #define DEBUG NONE in the same file .


All the other theoretical details or formulas have been mentioned in the paper.






