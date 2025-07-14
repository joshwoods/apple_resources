

- Kernel
- IOKit Fundamentals
- Data Types
- OSAction
-  SetAbortedHandler 

Instance Method

# SetAbortedHandler

Install a handler for the system to call when no other processes reference the action object.

DriverKitKernelDriverKit 19.0+macOS 10.15.2+

``` source
kern_return_t SetAbortedHandler(OSActionAbortedHandler handler);
```

## Parameters 

`handler`  

A handler block for the system to call. Specify `NULL` to remove the handler block from your action object.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See `Error Codes`.

## Discussion

The system calls your handler when no other objects reference the action object. If you want to keep the action object, use your handler to retain it. If you don't retain the object, the system releases it shortly after your handler returns.

## See Also

### Configuring the Action

+ Create

Creates a new action object and configures it with your custom target object and callback method.

- free

Performs any final cleanup for the action object.

