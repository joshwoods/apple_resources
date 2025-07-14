

- Kernel
- Hardware Families
- USB
-  IOUSBCompletionActionWithTimeStamp 

Type Alias

# IOUSBCompletionActionWithTimeStamp

The function that executes when the USB input/output request completes.

macOS 10.3+

``` source
typedef void (*IOUSBCompletionActionWithTimeStamp)(void *target, void *parameter, IOReturn status, UInt32 bufferSizeRemaining, AbsoluteTime timeStamp);
```

## Parameters 

`target`  

The target that the `IOUSBCompletion` structure specifies.

`parameter`  

The parameter that the `IOUSBCompletion` structure specifies.

`status`  

The completion status.

`bufferSizeRemaining`  

The bytes remaining to transfer.

`timeStamp`  

The time that the system processed the transaction.

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

IOUSBCompletionWithTimeStamp

A structure specifying action to perform when the USB input/output request completes.

