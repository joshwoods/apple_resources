

- Kernel
- Hardware Families
- USB
-  IOUSBHostCompletion 

# IOUSBHostCompletion

The structure that specifies the action to perform when the USB input/output request completes.

macOS 10.11+

``` source
struct IOUSBHostCompletion {
    ...
};
```

## Topics

### Getting the Properties

owner

A pointer to an object that owns the transfer.

action

The action to run when the input/output request completes.

parameter

A context pointer within the completion action.

## See Also

### Actions

IOUSBCompletionAction

A function the system calls when the USB input/output request completes.

IOUSBCompletion

The structure that specifies the action to perform when the USB input/output request completes.

IOUSBHostBundledCompletion

The structure that specifies the action to perform when a bulk USB input/output request completes.

IOUSBHostBundledCompletionAction

The function description for a USB host bundled completion action.

IOUSBHostCompletionAction

The function description for a USB host completion action.

IOUSBHostIsochronousCompletion

A structure describing the completion callback for an asynchronous isochronous operation.

IOUSBHostIsochronousCompletionAction

The function description for a USB host isochronous completion action.

IOUSBIsocCompletion

A structure specifying the action to perform when an isochronous USB input/output operation completes.

IOUSBIsocCompletionAction

The function that executes when the isochronous USB input/output request completes.

IOUSBLowLatencyIsocCompletion

The function that executes when the low-latency isochronous USB input/output request completes.

IOUSBLowLatencyIsocCompletionAction

The function that excutes when the low-latency isochronous USB input/output request completes.

IOUSBCompletionActionWithTimeStamp

The function that executes when the USB input/output request completes.

IOUSBCompletionWithTimeStamp

A structure specifying action to perform when the USB input/output request completes.

