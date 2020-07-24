List of projects on GitHub:

----
### Minfo (Minimal info)

Minfo is a tool for Linux Systems that displays a very succint overview of the OS.
Instead of running multiple commands to know various aspects of the OS, a single 
command can be used.

***It is written in Golang and tested on most Linux variants (Red Hat, Debian, & SUSE).***

```markdown
$ ./minfo
Minfo is a tool for displaying minimal system & network information.

Usage: minfo [OPTION]

  -h, --help          this message
  -V, --version       output version information
  -a, --all           displays all information
  -s, --sysinfo       displays system information
  -i, --ipinfo        displays ip information

$ ./minfo -a
System Info:
  CPU(s)                                  : 1
  CPU Model                               : Intel(R) Core(TM) i5 CPU M 480  @ 2.67GHz
  Architecture                            : x86-64
  Total Memory                            : 997956 kB / 974 MB / 0 GB
  Uptime                                  : 141.94 secs / 2 mins / 0 hours / 0 days
  Operating System                        : CentOS Linux 7 (Core)
  Kernel                                  : Linux 3.10.0-862.el7.x86_64
  System Type                             : Virtual Machine (vmware)
  Hostname                                : cos7
  Time Zone                               : America/Chicago (CDT, -0500)

IPv4 Info:
  interface                                 ip
  ---------                                 ---------
  ens33[0]                                : 192.168.229.20/24
  docker0[0]                              : 172.17.0.1/16

```

----
### sncalc (Subnet Calculator)

This tool takes an network IP address and CIDR value as input and provides useful 
information like the network address, broadcast address, host range in the network, 
and wildcard mask, among others. This website also provides a list of subnets possible 
with the IP & CIDR provided so that a large network can be subdivided into smaller 
manageable subnets.

***It is written in Golang and works on either Linux or Windows machines.***

```markdown
$ ./sncalc 192.168.1.0 26

IP Address                              : 192.168.1.0
Network Address                         : 192.168.1.0
Usable Host IP Range                    : 192.168.1.1 - 192.168.1.62
Broadcast Address                       : 192.168.1.63
Total Hosts per Subnet                  : 64   (2^unmasked bits) => (2^6)
Usable Hosts per Subnet                 : 62   (2^unmasked bits - 2) => (2^6 - 2)
Subnet Mask                             : 255.255.255.192
Wildcard Mask                           : 0.0.0.63
Binary Subnet Mask                      : 11111111.11111111.11111111.11000000
CIDR Notation                           : /26
Binary Octets                           : 11000000.10101000.00000001.00000000
Network Bits (total masked bits)        : 26
Hosts Bits (unmasked bits)              : 6

Number of Subnets: 4   (2^masked bits on 4th octet) => (2^2)
All 4 of the Possible /26 Networks for 192.168.1.* (valid subnets at 4th octet):
  Network Address      Usable Host Range                        Broadcast Address
  ---------------      -----------------                        -----------------
  192.168.1.0          192.168.1.1 - 192.168.1.62               192.168.1.63 [current]
  192.168.1.64         192.168.1.65 - 192.168.1.126             192.168.1.127
  192.168.1.128        192.168.1.129 - 192.168.1.190            192.168.1.191
  192.168.1.192        192.168.1.193 - 192.168.1.254            192.168.1.255

```

----
### Web Version of sncalc (Subnet Calculator)

This web application performs the same operations as the sncalc tool.

***It is written in HTML, CSS, Javascript, & Bootstrap.***

Click [HERE](https://sam1225.github.io/sncalc_web/) to use the app.
Click [HERE](https://github.com/sam1225/sncalc_web) to go to the repository.

----
----






