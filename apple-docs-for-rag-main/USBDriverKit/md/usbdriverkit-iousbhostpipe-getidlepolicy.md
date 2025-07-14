

- USBDriverKit
- IOUSBHostPipe
-  GetIdlePolicy 

Instance Method

# GetIdlePolicy

Retrieves the pipe’s current idle timeout.

DriverKit 19.0+

``` source
kern_return_t GetIdlePolicy(uint32_t * idleTimeoutMS);
```

## Parameters 

`idleTimeoutMS`  

A pointer to store the current idle timeout in milliseconds.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## See Also

### Managing the Pipe’s Idle Policy

SetIdlePolicy

Sets the pipe’s desired idle timeout.

