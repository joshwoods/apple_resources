

- Kernel
- Hardware Families
- 
  - Hardware Families
- Network
- IONetworkController
- TCP/IP
-  kChecksumTCPSum16 

# kChecksumTCPSum16

## Overview

The hardware has a simple checksum engine that can perform a TCP style ones complement sum of 16-bit words over a certain range of bytes in a packet. The hardware does not have the ability to scan for IP or TCP headers, and the driver must pass/get additional parameter(s) to or from the protocol stack to coordinate the checksumming effort.

