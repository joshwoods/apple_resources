

- Kernel
- Hardware Families
- USB
-  IOUSBHostIsochronousCompletionAction 

Type Alias

# IOUSBHostIsochronousCompletionAction

The function description for a USB host isochronous completion action.

macOS 10.11+

``` source
typedef void (*IOUSBHostIsochronousCompletionAction)(void *owner, void *parameter, IOReturn status, IOUSBHostIsochronousFrame *frameList);
```

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

IOUSBHostCompletion

The structure that specifies the action to perform when the USB input/output request completes.

IOUSBHostCompletionAction

The function description for a USB host completion action.

IOUSBHostIsochronousCompletion

A structure describing the completion callback for an asynchronous isochronous operation.

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

