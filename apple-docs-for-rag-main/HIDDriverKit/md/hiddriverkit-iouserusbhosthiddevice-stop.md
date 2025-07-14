

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  Stop 

Instance Method

# Stop

Stops the device service associated with the specified provider.

DriverKit 19.0+macOS

``` source
kern_return_t Stop(IOService * provider);
```

## Parameters 

`provider`  

The provider associated with the current service. This object is the same one that the system previously passed to your service’s Start method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Before terminating the object in `provider`, the system calls this method to stop the service associated with that object. Use your implementation of this method to stop all activity and put your driver in a quiescent state. Call `super` at the end of your implementation. After you call `super`, it is a programmer error to access the `provider` object.

## See Also

### Running the Service

init

Handles the basic initialization of the event service.

Start

Starts the current device service and associates it with the specified provider object.

handleStart

Performs any custom initialization associated with starting the device service.

free

Performs any final cleanup for the service.

