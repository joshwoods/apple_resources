

- DriverKit
- IODispatchSource
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

Don’t override this method or call it from your own code. Existing dispatch source objects implement this method internally and use it to generate new events.

