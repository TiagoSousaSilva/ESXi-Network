# Project_2
```
The ESXi project involved setting up a virtual network environment with four machines: Main, DHCPcli, DHCPFailover, and Windows.

Main served as the primary server, hosting multiple functionalities. It operated as a DHCP server, providing IP addresses to both DHCPcli and Windows machines located on different sides of the network topology. Additionally, Main hosted an email server, enabling six different users on the Windows machine to access email services through protocols like POP and SMTP.

DHCPcli was dedicated to serving as a web server, while Main facilitated this by functioning as a DNS server, translating the IP address of DHCPcli. This setup allowed the Windows machine to access DHCPcli's web server through a web browser. To enhance security, certificates were generated to enable an HTTPS site for secure communication.

In case Main experienced any downtime, DHCPFailover, another Debian system on the same network as the Windows machine, acted as a failover to ensure continuous availability and smooth operations.
```

The project demonstrates the configuration of virtual networks, server roles, email services, DNS, web servers, and failover mechanisms, all within the ESXi environment, with a specific focus on the interactions between Main, DHCPcli, DHCPFailover, and Windows.
