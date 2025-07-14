

- HIDDriverKit
- IOUserHIDDevice
-  Start 

Instance Method

# Start

Starts the device service and associates it with the specified provider object.

DriverKit 19.0+macOS

``` source
kern_return_t Start(IOService * provider);
```

## Parameters 

`provider`  

The provider object that matches the current device. Cast this object to the class you expect. The system retains this object for the duration of your `Start` method. The system continues to retain the object if your service starts successfully, releasing it only after calling your service’s Stop method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

After successfully matching the specified provider to your device, the system instantiates your device object and calls this method. Don’t override this method directly. Instead, implement your custom initialization code in the handleStart method.

This method calls newDeviceDescription and newReportDescriptor to retrieve information about your device. It then stores the results and starts your service.

## See Also

### Running the Service

handleStart

Performs any custom initialization associated with starting the device service.

