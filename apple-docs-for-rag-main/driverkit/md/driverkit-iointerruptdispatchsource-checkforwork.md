

- DriverKit
- IOInterruptDispatchSource
-  CheckForWork 

Instance Method

# CheckForWork

Checks for events to handle.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CheckForWork(bool synchronous);
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Don’t override this method or call it from your own code. The dispatch source uses this method internally to check for events.

## See Also

### Declaring Actions

InterruptOccurred

Executes custom code when an interrupt occurs.

IOInterruptDispatchSourcePayload

A private structure for an interrupt dispatch source.

