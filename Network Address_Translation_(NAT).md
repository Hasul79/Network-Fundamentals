# Network Address Translation (NAT)

<p>Network Address Translation(NAT) is a method that converts private IP addresses to public IP addresses. Since private IP addresses are non-routing IP addresses, these IP addresses cannot be used on the internet. These IP addresses allow communication in the local network only. Thanks to NAT, limited IPv4 addresses are used more sparingly. In addition, a kind of network segmentation is provided thanks to NAT. It is beneficial in controlling and securing the connections coming from outside the network into the network. In order to use the NAT method, a device with a gateway must perform packet routing. This device has a NAT table and IP address conversions are performed by looking at this table.</p>
<h2>NAT Advantages and Disadvantages</h2>
<p>Although NAT is often used as a solution to running out of IPv4 addresses, it also has some disadvantages. Some advantages and disadvantages can be seen in the table below.</p>

![nat-table-v2](https://github.com/Hasul79/Network-Fundamentals/assets/95657084/6419fad6-9562-49ff-a47c-10a99a5237e1)

<br/>

<h2>Example of NAT</h2>
<p>NAT is quite simple in nature. The simple working logic is shown in the picture below:</p>

![nat1](https://github.com/Hasul79/Network-Fundamentals/assets/95657084/c820f11b-cf10-4c6d-a49d-2a020be4a87d)

<p>When the device with an IP address of 10.6.1.2 goes to the Internet, it must first transmit the packet to the gateway device that provides the Internet output. The gateway device receiving the packet determines the network to which it will forward the packet and the destination address by looking at the information fields in the packet. After seeing that it has an IP address belonging to the Internet, it makes changes to the packet by using the information in the NAT table, in other words, it performs NAT conversion. After conversion, it forwards the packet to the next network device to forward the packet to the destination IP address. When the incoming response packet arrives, it redirects the packet to the relevant device in the internal network by performing the reverse of similar operations, and packet transmissions are performed together with NAT transformations.
In this part of the training, what NAT is, its advantages, disadvantages, and the simple working logic of NAT are discussed.</p>
