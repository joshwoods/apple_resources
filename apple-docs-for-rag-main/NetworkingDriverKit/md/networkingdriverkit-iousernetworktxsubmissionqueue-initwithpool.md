

- NetworkingDriverKit
- IOUserNetworkTxSubmissionQueue
-  initWithPool 

Instance Method

# initWithPool

DriverKit

``` source
bool initWithPool(IOUserNetworkPacketBufferPool * pool, IOUserNetworkServiceClass serviceClass, uint32_t capacity, IOUserNetworkPacketQueueId queueId, OSObject * target, QueryFreeSpaceAction freeSpaceAction, DequeueAction dequeueAction, void * refCon, IOOptionBits options);
```

