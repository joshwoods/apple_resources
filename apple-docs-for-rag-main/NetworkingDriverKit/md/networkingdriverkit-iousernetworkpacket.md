

- NetworkingDriverKit
-  IOUserNetworkPacket 

Class

# IOUserNetworkPacket

A network packet containing the data for your driver to process.

DriverKit

``` source
class IOUserNetworkPacket;
```

## Overview

An IOUserNetworkPacket contains meta information about a network packet being trasmitted to or from your device. You do not create network packets directly. Instead, you dequeue them from an appropriate submission queue, such as an IOUserNetworkRxSubmissionQueue. You a packet object to get the length of the packet data and the location of that data in its memory buffer, accommodating for any extra headroom bytes at the beginning of the packet.

## Topics

### Configuring the Network Packet

init

Initializes the network packet object.

free

Performs any final cleanup for the network packet.

### Configuring the Packet State Information

SetHeadroom

Changes the number of bytes to reserve at the front of the packet’s buffer to the specified value.

SetLinkHeaderLength

Changes the number of bytes to use for the link header to the specified value.

SetDataOffset

Changes the offset to the beginning of the packet’s data to the specified value.

SetDataLength

Changes the number of bytes of data in the packet to the specified value.

### Getting the Packet Information

GetHeadroom

Gets the number of bytes reserved at the front of the packet’s buffer.

GetLinkHeaderLength

Gets the number of bytes to use for the link header.

GetDataOffset

Gets the offset to the beginning of the packet’s data.

GetDataLength

Gets the number of bytes of data in the packet.

GetMemorySegmentOffset

Gets the offset to the beginning of the packet in the corresponding memory buffer.

### Getting the Packet’s Buffer Pool

GetPacketBufferPool

Gets the memory buffer that contains the pakcet.

### Instance Methods

clearTimestamp

getDataIOVirtualAddress

getDataLength

getDataOff

getDataOffset

getDataVirtualAddress

getExpiryTime

getLinkHeaderLength

getMSS

getMemorySegmentOffset

getPacketBufferPool

getRxChecksumInfo

getServiceClass

getTSOInfo

getTimestamp

getTraceID

getTxChecksumInfo

getTxCsumFlags

initWithPool

isLinkBroadcast

isLinkMulticast

isTimestampRequested

isTransportTrafficBackground

isTransportTrafficRealtime

prepareWithQueue

setCompletionStatus

setDataLength

setDataOff

setDataOffAndLen

setDataOffset

setDataOffsetAndLength

setIsLinkMulticast

setLROInfo

setLinkHeaderLength

setRxChecksumInfo

setTimestamp

setWakeFlag

traceEvent

### Type Methods

withPool

## Relationships

### Inherits From

- OSObject

## See Also

### Packet Management

IOUserNetworkPacketBufferPool

An object that manages the storage space for packets coming into and out of your driver.

IOUserNetworkPacketDirection

The direction in which the packet moves, relative to the device.

