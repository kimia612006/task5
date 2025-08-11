Task 5 – Wireshark Network Traffic Capture & Analysis

What I Did
I installed Wireshark, opened my active WiFi network interface, and started capturing live packets.
While the capture was running, I browsed a few websites and generated some internet activity.
After about a minute, I stopped the capture and began checking what protocols were flowing through my network.

What I Found
During the capture, I spotted different types of traffic:
BTDHT – This is BitTorrent's Distributed Hash Table protocol. I saw packets like Announce_peer and Get_peers, which are used for peertopeer communication.
TCP – The main transport protocol for reliable connections. I noticed HTTPS traffic on port 443.
IPv4 & IPv6 – Both versions of the Internet Protocol were in use. Examples include 23.208.65.107 (IPv4) and 2409:8a06:... (IPv6).

Observations
BTDHT packets showed my system was exchanging peer discovery messages.
TCP packets over port 443 were encrypted (HTTPS), so the content wasn’t readable.
My network is using both IPv4 and IPv6 at the same time (dualstack).

Tools Used
Wireshark – Free network protocol analyzer.

