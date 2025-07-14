

- HIDDriverKit
- IOUserHIDEventDriver
-  Start 

Instance Method

# Start

Starts the current event driver and associates it with the specified provider object.

DriverKit 19.0+macOS

``` source
kern_return_t Start(IOService * provider);
```

## Parameters 

`provider`  

The provider object that matches the current event driver. Cast this object to the class you expect. The system retains this object for the duration of your Start method. The system continues to retain the object if your driver starts successfully, releasing it only after calling your driver’s Stop method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

After successfully matching the specified provider to your event driver, the system instantiates your driver object and calls this method. Use this method to configure your custom data structures and any associated hardware. You might also store a reference to the provider object for later use. After you configure your event driver, call the RegisterService method to let the system know that your driver is running.

Always call `super` early in your implementation of this method. This method creates and parses the elements from the device’s initial report, making it easier to process future reports and dispatch events.

## See Also

### Running the Driver

init

Handles the basic initialization of the event service.

free

Performs any final cleanup for the service.

