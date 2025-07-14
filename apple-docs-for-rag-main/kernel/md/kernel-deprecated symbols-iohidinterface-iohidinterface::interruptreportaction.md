

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  IOHIDInterface::InterruptReportAction 

# IOHIDInterface::InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

``` source
typedef void ( *InterruptReportAction)(
   OSObject *target,
   AbsoluteTime timestamp,
   IOMemoryDescriptor *report,
   IOHIDReportType type,
   UInt32 reportID,
   void *refcon);
```

## Parameters 

`target`  

Pointer to your data object.

`timestamp`  

Time when the report was delivered.

`report`  

A memory descriptor that describes the report.

`reportType`  

The type of report.

`reportID`  

The ID of the report.

`refcon`  

void \* pointer to more data.

## Overview

This callback is set when calling IOHIDInterface::open.

## See Also

### Callbacks

CompletionAction

InterruptReportAction

Callback to handle an asynchronous report received from the HID device.

IOHIDInterface::CompletionAction

