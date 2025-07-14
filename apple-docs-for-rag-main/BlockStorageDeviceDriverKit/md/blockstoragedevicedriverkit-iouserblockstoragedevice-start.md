

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  Start 

Instance Method

# Start

Starts the current service and associates it with the specified provider.

DriverKit 21.0+

``` source
kern_return_t Start(IOService * provider);
```

## Parameters 

`provider`  

The provider object that matches the current service. Cast this object to the class you expect. The system retains this object for the duration of your `Start` method. The system continues to retain the object if your service starts successfully, releasing it only after calling your service’s Stop method.

## Return Value

A value that indicates the service-starting result. Return kIOReturnSuccess to inidicate success. To indicate a failure, see IOKit Constants for error definitions.

## Discussion

After successfully matching the specified `provider` to your driver’s service, the system instantiates your service object and calls this method. Use this method to configure your driver’s data structures and setup the associated hardware. You might also store a reference to the `provider` object for later use. After configuring your driver, call the RegisterService method to let the system know your service is running.

Always call `super` early in your implementation of this method.

## See Also

### Running the Service

init

Handles the basic initialization of the service.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

