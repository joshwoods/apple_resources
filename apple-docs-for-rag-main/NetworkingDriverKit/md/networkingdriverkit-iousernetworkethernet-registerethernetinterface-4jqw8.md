

- NetworkingDriverKit
- IOUserNetworkEthernet
-  RegisterEthernetInterface 

Instance Method

# RegisterEthernetInterface

Registers your driver with the networking stack.

DriverKit

``` source
kern_return_t RegisterEthernetInterface(IOUserNetworkMACAddress macAddress, IOUserNetworkPacketBufferPool * pool, IOUserNetworkPacketQueue * * queues, uint32_t queueCount);
```

## Parameters 

`macAddress`  

The MAC address of the hardware your driver supports.

`pool`  

The buffer pool you use to store incoming and outgoing packets.

`queues`  

An array containing the four queues you use to process incoming and outgoing network packets. This array must contain one queue each of types IOUserNetworkRxSubmissionQueue, IOUserNetworkRxCompletionQueue, IOUserNetworkTxSubmissionQueue, and IOUserNetworkTxCompletionQueue. The order of the queues in the array doesn’t matter.

`queueCount`  

The number of queues in the `queues` parameter. The `queues` parameter must contain 4 items.

## Discussion

Call this method toward the end of your Start method when your driver is ready to begin processing incoming and outgoing network packets.

## See Also

### Configuring the Driver Service

init

Handles the basic initialization of the service.

free

Performs any final cleanup for the service.

