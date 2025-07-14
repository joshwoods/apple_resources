

- NetworkingDriverKit
- IOUserNetworkRxCompletionQueue
-  Create 

Static Method

# Create

Creates a queue that you use to deliver packets received from your hardware device.

DriverKit

``` source
static kern_return_t Create(IOUserNetworkPacketBufferPool * pool, OSObject * owner, uint32_t capacity, uint32_t queueId, IODispatchQueue * dispatchQueue, IOUserNetworkRxCompletionQueue * * queue);
```

## Parameters 

`pool`  

The buffer pool containing the memory for the network packets. This parameter must not be `NULL`.

`owner`  

The object to use as the owner of the queue.

`capacity`  

The number of packets in the queue.

`queueId`  

An identifier for you to use to distinguish the queue from other queues. Specify `0` if you don’t use this parameter.

`dispatchQueue`  

The dispatch queue on which to execute tasks.

`queue`  

On return, the new queue object. It is a programmer error to specify `NULL` for this parameter.

## Return Value

`kIOReturnSuccess` on success, or another value if an error occurred.

## See Also

### Creating the Completion Queue

init

Initializes the packet submission queue.

free

Performs any final cleanup for the queue.

