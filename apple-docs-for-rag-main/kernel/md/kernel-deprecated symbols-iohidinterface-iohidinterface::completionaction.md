

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  IOHIDInterface::CompletionAction 

# IOHIDInterface::CompletionAction

``` source
typedef void ( *CompletionAction)(
   OSObject *target,
   void *refcon,
   IOReturn status,
   UInt32 bufferSizeRemaining);
```

## Parameters 

`target`  

`refcon`  

`status`  

Completion status.

`bufferSizeRemaining`  

Bytes left to be transferred.

## Overview

Function called when HID I/O completes.

## See Also

### Callbacks

CompletionAction

InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

IOHIDInterface::InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

