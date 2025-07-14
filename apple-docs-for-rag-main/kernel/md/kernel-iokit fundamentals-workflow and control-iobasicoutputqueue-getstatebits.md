

- Kernel
- IOKit Fundamentals
- Workflow and Control
- IOBasicOutputQueue
-  GetStateBits 

# GetStateBits

The bits in the value returned by getState().

``` source
enum {
   kStateRunning = 0x1,
   kStateOutputStalled = 0x2,
   kStateOutputActive = 0x4,
   kStateOutputServiceMask = 0xff00
};
```

## Topics

### Constants

kStateRunning

kStateStalled

kStateActive

