

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  CompletionAction 

# CompletionAction

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

InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

IOHIDInterface::CompletionAction

IOHIDInterface::InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

