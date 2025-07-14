

- NetworkingDriverKit
-  IOUserNetworkPacketBufferPool 

Class

# IOUserNetworkPacketBufferPool

An object that manages the storage space for packets coming into and out of your driver.

DriverKit

``` source
class IOUserNetworkPacketBufferPool;
```

## Overview

Create an IOUserNetworkPacketBufferPool during the initial setup of your driver and use it to store the packets that your driver transmits or receives. Every driver must have a packet buffer pool large enough to hold all of the packets in its transmit and receive queues. You allocate this pool early in the Start method of your IOUserNetworkEthernet service, and you deallocate that pool only after your service stops.

## Topics

### Creating a Buffer Pool

Create

Creates a new packet buffer pool object and allocates space for the specified number of packets.

init

Initializes the network packet buffer pool object.

free

Releases the resources owned by the network packet buffer pool object.

### Getting Pool Information

GetBufferCount

Returns the number of buffers associated with the network packet buffer pool.

GetPacketCount

Returns the number of network packets that the pool is capable of storing.

### Deallocating Packets

DeallocatePacket

Disposes of any resources associated with the packet and makes the packet available for reuse.

DeallocatePackets

Disposes of any resources associated with the specified packets and makes them available for reuse.

### Getting the Memory Block

CopyMemoryDescriptor

Returns a memory descriptor for the buffer pool’s contents.

### Instance Methods

allocatePacket

deallocatePacket

deallocatePackets

getPoolOwnerDevice

initWithName

newPacket

release

### Type Methods

CreateWithOptions

withName

## Relationships

### Inherits From

- OSObject

## See Also

### Packet Management

IOUserNetworkPacket

A network packet containing the data for your driver to process.

IOUserNetworkPacketDirection

The direction in which the packet moves, relative to the device.

