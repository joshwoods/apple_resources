

- NetworkingDriverKit
- IOUserNetworkRxSubmissionQueue
-  initWithPool 

Instance Method

# initWithPool

DriverKit

``` source
bool initWithPool(IOUserNetworkPacketBufferPool * pool, uint32_t capacity, uint32_t bufferCount, IOUserNetworkPacketQueueId queueId, OSObject * target, DequeueAction dequeueAction, void * refCon, IOOptionBits options);
```

