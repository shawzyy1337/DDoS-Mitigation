# Strategies for Reducing Severity of DDoS Attacks on Large-Scale Servers

This repository contains scripts and code snippets that can be used to reduce the likelihood and severity of DDoS attacks on large-scale servers. The strategies implemented include:

- Ignoring ICMP broadcasts: Installs a kernel parameter that ignores incoming ICMP broadcasts, and adds an IPTables rule to drop incoming ICMP packets.
- Dropping source routed packets: Installs a kernel parameter that prevents the server from accepting source routed packets.
- Enabling TCP SYN cookies: Installs a kernel parameter that enables TCP SYN cookies to help mitigate SYN flood attacks.
- Increasing the TCP SYN backlog: Increases the size of the SYN backlog to help mitigate SYN flood attacks.
- Decreasing TCP SYN-ACK retries: Decreases the number of retries when sending SYN-ACK packets to help mitigate SYN flood attacks.
- Enabling address spoofing protection: Installs a kernel parameter that enables protection against address spoofing attacks.
- Disabling SYN packet tracking: Installs a kernel parameter that prevents the server from tracking SYN packets.
- Dropping invalid packets: Adds an IPTables rule to drop packets that are marked as invalid.
- Installing bogus TCP flags: Adds several IPTables rules to drop packets with various combinations of invalid TCP flags.
And more...
# Usage
To use these strategies, clone this repository and run the appropriate script or code snippet on your server. Please note that these scripts may need to be run with root privileges.
