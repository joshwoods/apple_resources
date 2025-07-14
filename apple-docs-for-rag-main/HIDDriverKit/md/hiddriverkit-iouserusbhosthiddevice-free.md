

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  free 

Instance Method

# free

Performs any final cleanup for the service.

DriverKit 19.0+macOS

``` source
void free();
```

## Discussion

Use this method to perform any final cleanup of your device service, such as deallocating memory you allocated. The system calls this method at some point after it calls your service’s Stop method.

Always call `super` at the end of your custom implementation.

## See Also

### Running the Service

init

Handles the basic initialization of the event service.

Start

Starts the current device service and associates it with the specified provider object.

handleStart

Performs any custom initialization associated with starting the device service.

Stop

Stops the device service associated with the specified provider.

