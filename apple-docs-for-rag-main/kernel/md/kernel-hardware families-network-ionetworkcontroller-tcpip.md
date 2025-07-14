

- Kernel
- Hardware Families
- Network
- IONetworkController
-  TCP/IP 

# TCP/IP

TCP/IP checksums that may be supported by the hardware.

``` source
enum {
   kChecksumFamilyTCPIP = 0x00000001,
   kChecksumIP = 0x0001,
   kChecksumTCP = 0x0002,
   kChecksumUDP = 0x0004,
   kChecksumTCPIPv6 = 0x0020,
   kChecksumUDPIPv6 = 0x0040,
   kChecksumTCPNoPseudoHeader = 0x0100,
   kChecksumUDPNoPseudoHeader = 0x0200,
   kChecksumTCPSum16 = 0x1000
};
```

## Overview

Checksums

## Topics

### Constants

kChecksumFamilyTCPIP

kChecksumIP

kChecksumTCP

kChecksumUDP

kChecksumTCPIPv6

kChecksumUDPIPv6

kChecksumTCPNoPseudoHeader

kChecksumUDPNoPseudoHeader

kChecksumTCPSum16

