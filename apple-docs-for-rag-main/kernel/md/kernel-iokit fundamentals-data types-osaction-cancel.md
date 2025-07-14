

- Kernel
- IOKit Fundamentals
- Data Types
- OSAction
-  Cancel 

Instance Method

# Cancel

Cancels the execution of the action's callbacks.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
kern_return_t Cancel(OSActionCancelHandler handler);
```

## Parameters 

`handler`  

A handler block for the system to call after any in-flight callbacks finish executing.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See `Error Codes`.

## Discussion

After cancellation, you can only free the action object. You cannot reactivate it.

## See Also

### Ending the Action Early

- Aborted

Calls the abort handler of the action object.

OSActionAbortedHandler

The block to call before aborting an action object.

OSActionCancelHandler

The block to call after the successful cancellation of the action.

