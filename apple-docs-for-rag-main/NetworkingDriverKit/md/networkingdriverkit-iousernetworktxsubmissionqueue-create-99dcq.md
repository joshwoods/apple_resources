

- NetworkingDriverKit
- IOUserNetworkTxSubmissionQueue
-  Create 

Static Method

# Create

DriverKit 24.0+

``` source
static kern_return_t Create(IOUserNetworkPacketBufferPool * pool, OSObject * owner, IOUserNetworkServiceClass serviceClass, uint32_t capacity, uint32_t queueId, IODispatchQueue * dispatchQueue, IOUserNetworkTxSubmissionQueue * * queue);
```

