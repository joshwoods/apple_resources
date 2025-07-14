

- Kernel
- IOKit Fundamentals
- Memory
- IODMAController
-  queryDMACommand 

Instance Method

# queryDMACommand

macOS 10.11.4+

``` source
virtual IOReturn queryDMACommand(UInt32 dmaIndex, IODMACommand **dmaCommand, IOByteCount *transferCount, bool waitForIdle);
```

