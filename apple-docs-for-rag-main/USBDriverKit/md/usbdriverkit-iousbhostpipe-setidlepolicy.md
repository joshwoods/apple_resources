

- USBDriverKit
- IOUSBHostPipe
-  SetIdlePolicy 

Instance Method

# SetIdlePolicy

Sets the pipe’s desired idle timeout.

DriverKit 19.0+

``` source
kern_return_t SetIdlePolicy(uint32_t idleTimeoutMs);
```

## Parameters 

`idleTimeoutMs`  

The amount of time, in milliseconds, before an active transfer is considered idle. If 0, the pipe isn’t considered idle if there’s an I/O request enqueued.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

When a bulk or interrupt pipe is actively servicing an I/O request, it’s considered “busy” for the idle timeout value. For a more complete discussion of idle policies, refer to “Pausing IO” in `IOUSBHostFamily.h`.

## See Also

### Managing the Pipe’s Idle Policy

GetIdlePolicy

Retrieves the pipe’s current idle timeout.

