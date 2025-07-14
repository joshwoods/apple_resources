

- Kernel
- Hardware Families
- Network
-  IOPacketBufferConstraints 

Structure

# IOPacketBufferConstraints

macOS 10.6+

``` source
typedef struct IOPacketBufferConstraints {
    ...
} IOPacketBufferConstraints;
```

## Overview

Constraint parameters, specified by a driver, for the data buffer in a packet mbuf. This is observed by allocatePacket() to satisfy the stated requirements.

## Topics

### Instance Properties

alignLength

alignStart

reserved

## See Also

### Network Data

IONetworkData

An object that manages a fixed-size named buffer.

IONetworkMedium

An object that encapsulates information about a network medium (i.e. 10Base-T, or 100Base-T Full Duplex).

IOPacketQueue

Implements a bounded FIFO queue of mbuf packets.

