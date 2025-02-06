First off use Wireshark responsibly, monitoring network traffic without having permission can be considered illegal activity. Wireshark is a network analyzing tool that can filter, visualize, and capture packets from networks.
![image](https://github.com/user-attachments/assets/82c03646-70a7-4ce8-98db-3204db2e40ea)



 
I know looking at this can be overwhelming at a first glance, however once you understand what you looking at it will be a breeze.

First step to understanding this program is how to navigate the GUI.
 
You can adjust the size of the windows like you would any other tab to aid in focusing. This is the general packet hub in seeing the overall packets captured. In this window you can observe the number, time, source, destination, protocol, length, and info.

The number is simply the order of the packet captured and when selecting one you can see the other packets involved in the transfer of data.

The time shows how long it took to capture the packet.

The source shows the address of what device sent the packet

The destination shows where the packet was sent

The protocol shows what the purpose of the packet is

The length shows you well, the length of the packet in bytes, a byte is eight bits.

The info will give you a brief description of the packets contents


Second step to navigation is the packet details pane
 
In this window you will be able to dive deeper into each section of the packet to get a better depth than the general packet window. 

The other window you will see set out will be the byte window going over what each part in the packet detail window translates into hex and byte. Clicking on a section in the packet detail window will show you which specific part it correlates with.
 


With navigation out the way will dive into how to capture packets on a network

Second step
When you first open Wireshark you are greeted with this window
 
As seen in the bottom highlighted the next step is to select what network you want to begin capturing on, you can select more than one by using shift and left click, however I must emphasize again that you must have permission. A majority of universities when you agree to go to school is that you may not capture on their networks. At DePaul university doing so can lead to expulsion. So please only do so with permission. After selecting the desired network, you can click capture to begin. To stop capturing you can click the little fin in the top left corner or use ctrl + E(can also be used to start capture).


Third step
For more fine tuning of what you desire to capture you can use a filter next to the green book mark.

The next step in reading the packets you have captured are to analyze the packet details in the packet details window. As mentioned, it will allow you to dive into a greater depth of information on each packet. Showing the ethernet, Ip, TCP/UDP, and application layer. As I have been required to do in previous assignments, this window will be vital to answering any questions and allow you to comb through the information. 
Common filters: http → Show only HTTP packets. tcp.port == 443 → Display only HTTPS traffic. dns → View only DNS requests and responses.
 

Fourth step

To save what you have captured you must go to file and save as
 

While this covers basic navigation, some helpful steps to further breakdown what has been captured will be continued past this point.

Fifth step 
Color coding for faster navigation and analyzation. This can be done by going to view and then coloring rules.
 

Sixth step

The next step is to use protocol hierarchy to further get a traffic breakdown. Doing this will allow you to view the different percentages of different protocols aiding in observing any traffic spikes. 
 

Seventh step
The next step is to identify conversations between devices. This simply shows conversations between Ips and is a good tool for identifying conversations.
 

Eighth step

The last step I will be providing to aid in conversation breakdown will be the usage of the expert info window. This window will allow you to navigate errors caught in the capture. This can be viewed by going to analyze and then expert info.
 

This is all I will be covering in this simple guide on how to navigate, capture, and read in Wireshark. You will be able to navigate most assignments assigned and build fluency.  
