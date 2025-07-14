

- DriverKit
-  QUEUENAME 

Macro

# QUEUENAME

Tells the system to execute a method on the dispatch queue with the specified name.

DriverKitiOSiPadOSmacOS

``` source
#define QUEUENAME(name)
```

## Parameters 

`name`  

The name of the instance variable that contains an IODispatchQueue object.

## Discussion

Add this macro to the end of your method declaration in the `.iig` file of your class. When this macro is present, DriverKit executes your method on the dispatch queue with the specified name. You must register the dispatch queues your driver uses by calling the SetDispatchQueue method as part of your driver’s configuration. The following code listing shows the declaration of a method that handles asynchronous I/O for a USB pipe. DriverKit executes the method on a previously registered dispatch queue with the name `tx_pipe_dq`.

```
TxComplete (OSAction            *action,
            uint32_t             ioCompletionIndex,
            uint32_t             ioCompletionCount,
            const uint32_t       actualByteCountArray[kIOUSBHostPipeBundlingMax],
            int                  actualByteCountArrayCount,
            const kern_return_t  statusArray[kIOUSBHostPipeBundlingMax],
            int                  statusArrayCount) TYPE(IOUSBHostPipe::CompleteAsyncIOBundled) QUEUENAME(tx_pipe_dq);

```

## See Also

### Runtime support

OSDynamicCast

Casts an object safely to the specified type, if possible.

OSRequiredCast

Casts the object to the specified type, stopping the process if the object isn’t of the correct type.

IMPL

Tells the system that the superclass implementation of this method runs in the kernel.

TYPE

Annotates a method declaration to indicate that it conforms to an existing method signature.

SUPERDISPATCH

Tells the system to execute the superclass’ implementation of the current method in the kernel.

IIG_KERNEL

Tells the system that the class or method runs inside the kernel.

LOCAL

Tells the system that the method runs locally in the driver extension’s process space.

LOCALONLY

Tells the system that the class or method runs locally in the driver extension’s process space.

Error Codes

Determine the reason an operation fails.

C++ Runtime Support

Examine low-level types that DriverKit uses to support kernel-level operations.

