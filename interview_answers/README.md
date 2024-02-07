1. User says their internet is slow and that it takes ages to get to websites. What steps would you do to troubleshoot?

    Test the internet speed online.
    Check and secure cable connections.
    Restart the modem and router.
    Move closer to the Wi-Fi router or reduce signal interference.
    Run a virus scan on the device.

2. Tell me five ways to find the current date and time on a Linux system.

    Use the date command.
    Run timedatectl for date, time, and timezone.
    Check hwclock for the hardware clock.
    Look at /etc/localtime for timezone info.
    Some systems support the clock command.

3. How would you delete a file called -f on a Linux system?

    Use rm -- -f to delete the file named -f.

4. Can you explain the difference between a hub, a router, and a switch?

    Hub: Connects devices in a network, sending data to all devices.
    Switch: Connects devices smarter than a hub by sending data only to the intended device.
    Router: Connects multiple networks, directing data to its correct destination, and can provide Wi-Fi.

4. Can you explain the difference between a hub, a router, and a switch.

A hub connects multiple networks or computers together. A router does the same except it determines the best way to route data packets. A switch is a like a routers but uses MAC addresses to only send data to the device that needs it. 

5. What are the layers of the OSI model and describe each one?

	There are seven model layers:
	Physical: Hardware connections and physical data transfers.
	Data link: Manages between physical network nodes including MAC addresses. 
	Transport: End-to -End data transfer
	Session: Manages network sessions. 
	Network: Finds best way to move data through device addressing.
	Application: Manages applications services.
	Presentation: Transform data to application layer while dealing with compression and encryption.   

6. How would you find a device on a network?

Ping, traceroute, or use network scanning tools.

7. How does traceroute work? How is it different from ping?

Traceroute identifies the each hop taken by data packets from the source to the destination. Ping measures the response time it takes to do a roundtrip of data transmission and network connectivity. Ping: Measures the round-trip time for messages sent from the source to a destination and back. Mainly used to check network connectivity and response time.

8. What is ping?

Ping is a diagnostic that measures the response time it takes to do a roundtrip of data transmission and network connectivity.

9. Draw an entire network (very broad, but will allow you to show everything you know about one)
![simple-network-diagram-template](https://github.com/Oueael/Tech-Interview-Questions/assets/125812553/74ccc6c4-3c80-43e0-b2ca-a944b5536700)

10. What is DHCP? How does it work? What is assigned to the computer that requested an address?
DHCP stands for Dynamic Host Configuration Protocol which automatically assigns IP addresses to devices on a network.

11. What is ARP?
ARP stands for Address Resolution Protocol and resolves an IP address to a MAC address and is used to find a physical address of a network node. 

12. How does a switch work?
Switches use MAC addresses to efficiently forward data to the correct device in a network.

13. What are some ways you can kill a program that is not responding? (think of the command line as well)
. Windows: Press Ctrl+Shift+Esc to open Task Manager and end the task. Use taskkill in command line.
     Mac: Press Cmd+Opt+Esc and force quit. Use kill or killall in terminal.
     Linux: Use kill or killall in terminal.

14. On a Linux machine, how would you find the drive you just plugged in? How would you mount it?

Use lsblk to see the drive. Create a mount point (mkdir /media/newdrive) and mount the drive (mount /dev/sdx1 /media/newdrive) to mount it.

15. With the kill command, what does -9 do (kill -9)? How is it different than kill -11?

kill -9 forces a program to stop immediately. kill -11 stops a program due to code error.

16. What is DNS?

16. DNS(Domain Name System) turns website names into IP addresses that computers understand.

17. On a Mac, what are some ways you can transfer data from one computer to another?

17. AirDrop, iCloud, USB, or network file sharing.

18. What do the PRAM and SMC reset do? What do each reset?

PRAM resets the Parameter RAM, clearing settings like sound volume and time zone. SMC resets the System Management Controller, responsible for issues related to power, battery, fans, and other system performance.

19. Say that I opened my browser and went to www.google.com. Describe what exactly happens in order for the page to display in my browser?

Your browser initiates a DNS lookup to find the IP address of www.google.com then sends an HTTP request to Google's server. The server then responds with the HTML, CSS, and JavaScript of the page. Your browser then renders the page content, making additional requests for objects like images and executing JavaScript code.

20. What is an inode? What metadata does it contain?

An inode is a data structure on a filesystem on Unix-like systems. It stores information about a filesystem object but does not contain the data itself or the filename. Metadata in an inode includes the file size, device ID, user ID, group ID, file mode, timestamps, and link count.

21. What is the difference between a hard link and a soft link (symlink)?

A hard link is a direct reference to the file's inode, acting indistinguishably from the file itself. A symlink is a pointer to a file name; it's a separate file that redirects to another file or directory.

22. What is the Windows registry? How does linux do the same thing? Mac?

The Windows Registry is a database storing low-level settings for the OS and applications. Linux uses configuration files (often found in /etc) and directories for this purpose. macOS utilizes both configuration files and a database similar to the Registry called plist files.

23. What is the bootup process of a machine of your choice?

For a Linux machine, the boot process typically involves the BIOS/UEFI initializing hardware, then booting from a storage device. It loads the bootloader (like GRUB) which then loads the kernel. The kernel initializes the system and starts the init process, which brings up the system in user-space.

24. What are the differences between 802.11 a, b, g, and n?

'a' uses 5GHz (faster speeds, shorter range), 'b' and 'g' use 2.4GHz ('b' is slower, 'g' is faster), and 'n' can use both frequencies.

25. What is in an IP header? TCP Header?

An IP header includes source and destination addresses and other data for routing. A TCP header includes ports, sequence numbers, and flags for data management.

26. What is the difference between a public IP and a private IP?

Public IPs are unique across the internet, while private IPs are local within networks and not globally unique.

27. What port is SMTP? Is there more than one port used for SMTP?

SMTP usually uses port 25 for non-secure connections and port 465 for secure SSL connections. There's also port 587 for secure submissions.

28. What is an MX record?

An MX record is a DNS record that specifies the mail server responsible for accepting email on behalf of a domain.

29. Describe the TCP Handshake.

1. the sender sends a SYN message. 2. The receiver responds with SYN-ACK. 3. The sender replies with ACK, establishing a connection.

30. What is the difference between TCP and UDP?

TCP is reliable with error checking, awhile UDP is faster but less reliable, without error checking.

31. A user has a machine that shows no output on the monitor. How to troubleshoot?

Check cable connections, monitor power, try different monitors or cables.

32. How do you define the following types of malware: a worm, a trojan, a rootkit?

A worm self-replicates to spread, a trojan disguises itself as legitimate software, and a rootkit hides its presence while maintaining privileged access.

33. How are ICMP packets denoted in the IP header? How are ICMP echo and reply denoted?

ICMP packets are identified by the protocol field in the IP header. Echo requests and replies are differentiated by their type and code fields.

34. What routing protocol do you think Google uses and why?

Google likely uses advanced routing protocols that can handle large amounts of data efficiently, such as BGP (Border Gateway Protocol). BGP helps manage how packets of data are routed across the internet, choosing the best paths for data to travel quickly and reliably, which is crucial for a massive network like Google's.

35. You have 2 Linux machines. How would you copy host A's disk0 to host B's disk1 and verify it copied correctly?

You can use the dd command to copy the entire disk from host A to host B over a network connection, then use ssh for the transfer. To verify it copied correctly, you can compare checksums of both disks using a command like md5sum or sha256sum. This ensures both disks have the exact same data.

36. A user with a Windows laptop says that whenever they try to visit a particular website they instead see some strange Russian website they're not expecting. How would you troubleshoot this?

First, check the browser's settings and extensions to ensure nothing is redirecting the user. Then, inspect the system for malware or viruses that could cause redirects. Finally, check the hosts file for any unusual entries that might redirect websites.

37. In Linux, you want to unmount a filesystem but it is in use. Can you fix this without rebooting the machine?

Yes, you can use the lsof or fuser commands to find out what processes are using the filesystem. Then, you can safely stop those processes or services. After stopping them, you should be able to unmount the filesystem without rebooting.

38. What is RAID? Describe RAID 0, 1, 5, 6, and 10

    RAID stands for Redundant Array of Independent Disks. It's a way to store the same data in different places on multiple hard disks to protect data in the case of a drive failure.
        RAID 0 splits data evenly across two or more disks with no redundancy, offering improved performance but no fault tolerance.
        RAID 1 mirrors data across two or more disks, providing high fault tolerance.
        RAID 5 distributes data and parity information across three or more disks, offering a good balance of performance, storage capacity, and fault tolerance.
        RAID 6 is similar to RAID 5 but can withstand two disks failing simultaneously thanks to extra parity data.
        RAID 10 combines mirroring and striping to provide both high performance and fault tolerance by using at least four disks.

39-40. Your machine needs to send data to a host with an IP address on the same LAN. How does it specify the address the data should go to? Be prepared to talk about any acronyms you mention.

    It uses the ARP (Address Resolution Protocol) to find out the MAC (Media Access Control) address that corresponds to the IP address in the same LAN. The data is then sent to that specific MAC address.

41. How do you start a website using Apache?

    Install Apache on your server, then configure its settings to point to your website's files by editing the Apache configuration files. Place your website files in the designated directory, and restart Apache to make your site live.

42. You are a new consultant at a company and you are to give the company new internet. What up and down speeds would you provide and why?

    It depends on the company's needs. For most companies, a high-speed internet connection ranging from 100 Mbps to 1 Gbps would be sufficient, considering factors like the number of users, type of business, and how much video conferencing, file downloading/uploading, and online applications they use. The goal is to ensure smooth, uninterrupted internet access for all business operations.

43. What is OWFS?

    OWFS stands for One-Wire File System. It's a way to access and control devices on a one-wire network as if they were files in a directory. This makes it easier to interact with sensors and other devices on a one-wire network, commonly used in home automation and data collection applications.

44. What is Journaling? Why is it useful?

    Journaling is a feature used by some file systems to keep track of changes not yet committed to the file system's main part. It's useful because it helps protect the integrity of the data by allowing the system to recover more quickly and accurately in case of a power failure or system crash by replaying or ignoring uncommitted changes.

45. What is HTTPS? How does it work?

    HTTPS stands for HyperText Transfer Protocol Secure. It's the secure version of HTTP, where communications between your browser and the website are encrypted. This is achieved through the use of SSL/TLS protocols, which ensure that any data transferred cannot be intercepted or read by others.

46. How do private and public keys work?

    Private and public keys are part of encryption systems, like RSA, used for secure communication. The public key can be shared with anyone and is used to encrypt messages. The private key is kept secret and is used to decrypt messages encrypted with the public key. This ensures that only the holder of the private key can read the message.

47. Does DNS use TCP or UDP? Why?

    DNS (Domain Name System) primarily uses UDP (User Datagram Protocol) for its queries due to the protocol's speed and efficiency with small amounts of data. However, it can use TCP (Transmission Control Protocol) for larger queries or zone transfers, which require reliability and error-checking.

48. What is QoS?

    QoS stands for Quality of Service. It's a technology that manages data traffic to reduce packet loss, latency and jitter on a network. QoS prioritizes certain types of traffic (like video conferencing) over less critical traffic (like file downloads), ensuring that important applications have the bandwidth they need to perform well.

49. What is a VLAN?

    A VLAN (Virtual Local Area Network) is a method to create separate networks on the same physical hardware for better management, security, and performance. It allows network administrators to segment networks without requiring additional hardware, making it easier to manage traffic and enforce policies.

50. What is TLS?

    TLS stands for Transport Layer Security. It's a protocol that provides encryption and secure communication over the internet, ensuring that data between two communicating parties is private and reliable. It's widely used in web browsers and other applications that require data to be securely exchanged.

51. What is ICMP?

    ICMP stands for Internet Control Message Protocol. It's used by network devices, like routers, to send error messages indicating, for example, that a requested service is not available or a router could not be reached, helping in diagnosing network communication issues.

52. What is a fork bomb?

    A fork bomb is a type of attack against a system that involves creating a large number of processes very quickly to saturate the available space in the list of processes, causing the system to slow down or crash due to resource exhaustion.

53. How would you test if a port is open on a remote server?

    You can use tools like telnet, nc (netcat), or nmap to test if a port is open on a remote server. These tools allow you to attempt a connection to the specified port on the server. If the connection is successful, the port is open.

54. You opened a port on a server, but from the outside, you cannot connect to that port. What might the problem be?

    The issue could be due to a firewall blocking the port on the server or along the network path. Another possibility is that the service meant to listen on that port isn't running or is configured incorrectly. Also, network configuration issues like incorrect routing or IP address settings could prevent access.

55. A fellow technician says that a Windows machine they're working on has an IP address of 169.254.101.6, and asks you to help him troubleshoot. What do you do?

    An IP address starting with 169.254 indicates that the machine is using Automatic Private IP Addressing (APIPA) because it couldn't obtain an IP address from a DHCP server. Check the network connection, ensure the DHCP server is operational, and try renewing the IP address on the Windows machine using the ipconfig /renew command.

56. What are IPTables? What are the different things you can do with them?

    IPTables is a command-line firewall utility in Linux that allows you to define rules for how incoming and outgoing traffic should be handled. With IPTables, you can filter traffic, redirect traffic, allow or block specific ports or IP addresses, and protect the system from unauthorized access.

57. On a Linux machine, how can you spin up a webserver? What is a vhost? Where do the configuration files live?

    To spin up a webserver on Linux, you can install web server software like Apache or Nginx using package managers (apt for Debian/Ubuntu, yum for CentOS). A virtual host (vhost) allows a single web server to serve multiple websites. Configuration files for Apache typically live in /etc/apache2/sites-available on Debian/Ubuntu systems and /etc/httpd/conf.d on CentOS systems. For Nginx, they're usually in /etc/nginx/sites-available.

58. Name a few HTTP requests.

    Some common HTTP requests include GET (retrieve data), POST (submit data to be processed), PUT (update data), DELETE (remove data), and HEAD (retrieve headers for a specific resource).

59. List some ports and define what they are used for.

    Port 80: Used for HTTP, web traffic.
    Port 443: Used for HTTPS, secure web traffic.
    Port 22: Used for SSH, secure shell access.
    Port 21: Used for FTP, file transfers.
    Port 25: Used for SMTP, sending emails.

60. What command would you use to list the number of threads for a running process?

    On Linux, you can use ps -o nlwp <pid> where <pid> is the Process ID, to list the number of threads. nlwp stands for number of lightweight processes (threads).

61. How would you find the system load average WITHOUT causing more load?

    You can use the uptime or top command. Both provide the system load average without adding significant load to the system themselves.

62. What are some of the default Linux system variables?

    Some default Linux environment variables include PATH (directories to search for executable files), HOME (the current user's home directory), USER (the name of the current user), and SHELL (the path to the current user's shell).

63. What is garbage collection?

    Garbage collection is a form of automatic memory management. The garbage collector attempts to reclaim memory occupied by objects that are no longer in use by the program, preventing memory leaks and helping ensure efficient use of memory.

64. Using bash, how would you output a specific column in a file?

    Use the cut command. For example, cut -d',' -f2 file.csv outputs the second column of a CSV file.

65. What's the difference between BOOTP and DHCP?

    BOOTP is an older protocol that assigns IP addresses from a pool but doesn't support dynamic reallocation. DHCP, newer and more flexible, allows dynamic, automatic allocation and management of IP addresses and other network settings.

66. What is Immutable Infrastructure? How does it differ from Mutable Infrastructure and what are some advantages of having an Immutable Infrastructure?

    Immutable Infrastructure means once deployed, components are never updated or changed; if changes are needed, you replace them with new ones. Mutable Infrastructure allows updates/changes after deployment. Advantages of Immutable Infrastructure include predictability, reliability, and simpler rollback processes.

67. Name a few data structures.

    Arrays, Linked Lists, Stacks, Queues, Trees, Graphs, Hash Tables.

68. What tool would you use to sniff DNS traffic?

    Wireshark or tcpdump can be used to capture and analyze DNS traffic.

69. What tool would you use to view disk IO?

    iotop or iostat can be used to monitor disk IO on Linux systems.

70. What is a CDN?

    A Content Delivery Network (CDN) is a network of servers distributed geographically to reduce latency by serving web content from a location closer to the user.

71. What is Puppet, Ansible, Chef, SaltStack and what are they used for?

    These are configuration management and orchestration tools used to automate the setup, deployment, and management of servers and applications. Puppet, Chef, and SaltStack use a master-agent model, while Ansible uses a masterless model.

72. What is the difference between git pull and git fetch?

    git fetch downloads changes from a remote repository to your local repo without merging them, while git pull fetches changes and then automatically merges them into your current branch.

73. What does git rebase do?

    git rebase is used to apply changes from one branch onto another, effectively moving the base of the current branch to the tip of another branch. This is often used to maintain a clean project history by integrating changes without creating merge commits.

74. Write a Puppet class to include the apache module and add the attributes for hostname and www_root. Set www_root to /mnt/mount.

puppet

class webserver {
  class { 'apache':
    www_root => '/mnt/mount',
    # Assuming hostname is managed via a different parameter or fact.
  }
}

75. The node that has /mnt/root begins having issues. The /mnt/root is an NFS mount and a process is using the mount. What commands can you use to determine what is using the mount?

    Use lsof | grep /mnt/root or fuser -m /mnt/root to identify processes using the mount.

76. Let's say you have 5 web hosts behind HAproxy. One of the servers started experiencing issues. What would you do?

    Initially, I would temporarily remove or disable the problematic server in the HAproxy configuration to mitigate impact on the service. Then, I'd investigate logs and system metrics on the affected server to diagnose the issue.

77. From the last question, how would you troubleshoot the node having issues?

    Check server logs (access logs, error logs), system health (CPU, memory, disk usage), and application-specific metrics. Use tools like top, netstat, and application performance monitoring (APM) solutions for deeper insights.

78. You have a border router and behind the router is an HAproxy endpoint serving 5 web nodes behind it. All of a sudden, you begin getting 10Gbps traffic to the HAproxy node and it becomes unresponsive. What do you do?

    Implement rate limiting or DDoS protection rules on the border router or use external DDoS mitigation services. You might also redistribute traffic, if possible, and analyze the traffic pattern to block malicious sources.

79. What is a Puppet module? If you needed to make changes to a module, what can you do?

    A Puppet module is a collection of manifests and data (such as files, templates, and facts) defining a specific configuration to manage resources. To modify a module, you can edit its manifests or data files directly, or override its parameters in your node or class definitions.

80. What are ports and port numbers to DNS, FTP, and DHCP?

    DNS: 53 (TCP/UDP), FTP: 21 for command/control (TCP), 20 for data transfer (TCP), DHCP: 67 for server and 68 for client (UDP).

81. What Linux command would you use to limit administration access?

    Use visudo to edit the /etc/sudoers file safely, defining who has sudo privileges and to what extent.

82. What is ransomware?

    Ransomware is malicious software designed to block access to a computer system or encrypt files until a sum of money (ransom) is paid.

83. Explain WannaCry

    WannaCry is a ransomware attack that spread globally in May 2017, exploiting a vulnerability in Microsoft Windows OS to encrypt files on infected machines, demanding ransom payments in Bitcoin for decryption keys.

84. How do you find out the latest exploits and news in the industry?

    Stay informed through cybersecurity websites (e.g., CVE databases, SecurityFocus), forums, newsletters, social media (e.g., Twitter accounts of security researchers), and professional networks. Attending security conferences and webinars also helps.

85. Which 3-part handshake protocol is used to establish a connection?

    TCP (Transmission Control Protocol) uses a three-way handshake (SYN, SYN-ACK, ACK) to establish a connection.

86. Name the IP address ranges for the different classes and what their subnet masks were.

    Class  1.0.0.0 to 126.0.0.0, Subnet Mask: 255.0.0.0
    Class B: 128.0.0.0 to 191.255.0.0, Subnet Mask: 255.255.0.0
    Class C: 192.0.0.0 to 223.255.255.0, Subnet Mask: 255.255.255.0

87. Name the private IP addresses, their subnet masks, and their CIDR.

    Class  10.0.0.0 to 10.255.255.255, Subnet Mask: 255.0.0.0, CIDR: 10.0.0.0/8
    Class B: 172.16.0.0 to 172.31.255.255, Subnet Mask: 255.240.0.0, CIDR: 172.16.0.0/12
    Class C: 192.168.0.0 to 192.168.255.255, Subnet Mask: 255.255.0.0, CIDR: 192.168.0.0/16

88. What is CIDR?

    Classless Inter-Domain Routing (CIDR) is a method for allocating IP addresses and IP routing that replaces the old system based on classes A, B, and C. It allows for more efficient allocation of IP addresses.

89. Which security method helps block and prevent ports from being accessed?

    Firewalls help block unauthorized access to or from private networks, including managing port access.

90. What prevents a network from intrusion?

    Intrusion Prevention Systems (IPS), firewalls, regular software updates, strong password policies, and network monitoring tools are used to prevent unauthorized access and intrusions.

91. What is an injection attack?

    An injection attack involves inserting malicious code into a program or query that executes unauthorized commands in a system, database, or application (e.g., SQL injection, script injection).

92. How do you read Wireshark and an IDS/IPS scan paper for intrusion scans and how/why the intrusion occurred?

    Analyze packet captures in Wireshark for suspicious activity, such as unusual protocols, ports, or traffic volumes. Review IDS/IPS logs for alerts on known attack signatures or anomalies. Correlate this data with known vulnerabilities or exploit methods to understand how and why an intrusion may have occurred.
