

- HIDDriverKit
- IOUserUSBHostHIDDevice
-  Start 

Instance Method

# Start

Starts the current device service and associates it with the specified provider object.

DriverKit 19.0+macOS

``` source
kern_return_t Start(IOService * provider);
```

## Parameters 

`provider`  

The provider object that matches the current service. This method requires that the provider be an IOUSBHostInterface object, and returns an error if it isn’t. The system retains this object for the duration of the `Start` method. The system continues to retain the object if your service starts successfully, releasing it only after calling your service’s Stop method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

After successfully matching the specified provider to your device, the system instantiates your device object and calls this method. This method configures the USB device and sets up the pipes needed for communication.

Don’t override this method directly. Instead, implement your custom initialization code in the handleStart method.

## See Also

### Running the Service

init

Handles the basic initialization of the event service.

handleStart

Performs any custom initialization associated with starting the device service.

Stop

Stops the device service associated with the specified provider.

free

Performs any final cleanup for the service.

