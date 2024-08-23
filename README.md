# moyai.dev
Moyai Services, moyai.dev, is a commerical website designed to host goods and services. https://moyai.dev

## About
Moyai leverages a robust technology stack, incorporating HTML5, CSS, PHP, and JavaScript for its core functionality. The application is containerized using Docker and deployed within a Proxmox virtualization environment. The underlying infrastructure utilizes a Debian-based Linux distribution as the host operating system for the Docker container.

To bolster security and ensure robust network isolation, a VPN client has been implemented on the Debian system, utilizing a static IP configuration. Comprehensive firewall rules have been established at both the Proxmox and VPN client levels, effectively restricting incoming traffic from the ISP's public IP address as well as the VPN's static public IP.
Additionally, the virtual machine has been configured to prevent any communication with devices on the local area network (LAN) or the VPN network, further enhancing security measures. To protect data transmitted between the web server and its clients, SSL has been integrated, utilizing Let's Encrypt for deployment. This implementation not only secures communications but also fosters trust with users accessing the web server. <em>The client certificate comes from CloudFlare, not Let's Encrypt.</em>

Traffic management is handled by Nginx, a high-performance reverse proxy server, which is also containerized and runs alongside the main application. This setup ensures efficient request routing and load balancing. The domain infrastructure, including moyai.dev and its subdomains, is managed through CloudFlare's domain registration and DNS services.

This architecture demonstrates a well-designed, security-focused deployment strategy that prioritizes isolation, access control, and scalability.

## List of Sub-Domains
I have compiled a list of all websites currently hosted under and associated with the moyai.dev domain. This list is provided below.
<ul>
  <li>https://next.moyai.dev</li> | NextCloud
</ul>

## Site Version
I will indicate the year followed by the revision count. For example, in the year 2024, including this current revision, it would be denoted as <b><em>2024.4</em></b>.
