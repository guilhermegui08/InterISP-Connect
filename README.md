# InterISP-Connect
InterISP Connect is a comprehensive project focused on planning, designing, configuring, and documenting a network scenario involving multiple Internet Service Providers (ISPs) interconnected to provide connectivity to a corporate client. Leveraging the capabilities of the GNS3 application, the project encompasses tasks related to network design, configuration, and documentation to ensure seamless connectivity and robust network performance for the client's enterprise needs.
![topologia](https://github.com/guilhermegui08/InterISP-Connect/assets/112128696/580bb7dc-39fa-4edc-8fe9-37cf5ea7b013)


 ## Network Optimization and Design Considerations

1. **Addressing Optimization:**
   - Utilize link-local addresses on all interfaces with IPv6 to meet network requirements efficiently.

2. **IGP Domain Configuration for ISP Tier 1:**
   - Implement OSPFv3 in a multi-area environment with sufficient routers to support diverse area types.

3. **Traffic Routing from ISPs Tier 3:**
   - Direct traffic from Tier 3 ISPs through Tier 2A, with Tier 2B used as a backup in case of Tier 2A link failure.

4. **Redundancy and Load Balancing:**
   - Ensure redundant and parallel use of links between Tier 3 and Tier 2, enhancing network resilience.

5. **Preferred Links in Tier 1 Connections:**
   - Define preferred links in Tier 1 connections to either Tier 2, optimizing network performance.

6. **BGP Implementation in ISP Tier 1:**
   - Implement BGP with reduced iBGP connections to manage router growth efficiently, prioritizing confederations.

7. **Quality of Service (QoS) in Tier 2A:**
   - Implement QoS in Tier 2A to prioritize network traffic and enhance service quality.

8. **Design Considerations for Corporate Client:**
   - Utilize private addressing for the corporate client.
   - Implement IPv4 addressing for the corporate client.
   - Connect company sites via L3 VPN over MPLS technology.
   - Consider identified protocols for branch connectivity with operator PE routers.
   - Ensure internet connectivity for internal equipment through the headquarters router.
   - Implement QoS for the corporate client to manage network traffic effectively.
