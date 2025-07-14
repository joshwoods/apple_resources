

- Kernel
- Hardware Families
- 
  - Hardware Families
- Network
- IONetworkController
- TCP/IP
-  kChecksumUDPNoPseudoHeader 

# kChecksumUDPNoPseudoHeader

## Overview

A UDP checksum that covers the UDP header and the UDP data, but the pseudo header is not included in the checksum computation. A partial 16-bit checksum value must be provided to allow the protocol stacks to calculate and verify the final checksum. This type of checksum is not currently supported on the output path.

