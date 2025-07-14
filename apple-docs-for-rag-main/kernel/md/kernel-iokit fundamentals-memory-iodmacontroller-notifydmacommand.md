

- Kernel
- IOKit Fundamentals
- Memory
- IODMAController
-  notifyDMACommand 

Instance Method

# notifyDMACommand

macOS 10.11.4+

``` source
virtual void notifyDMACommand(IODMAEventSource *dmaES, IODMACommand *dmaCommand, IOReturn status, IOByteCount actualByteCount, AbsoluteTime timeStamp);
```

