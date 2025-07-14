

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  Stop 

Instance Method

# Stop

Stops the service associated with the specified provider.

DriverKit 21.0+

``` source
kern_return_t Stop(IOService * provider);
```

## Parameters 

`provider`  

The provider associated with the current service. This object is the same one that the system previously passed to your service’s Start method.

## Return Value

A value that indicates the service-stopping result. Return kIOReturnSuccess to inidicate success. To indicate a failure, see IOKit Constants for error definitions.

## Discussion

Before terminating the object in `provider`, the system calls this method to stop the service associated with that object. Use your implementation of this method to stop all activity and put your driver in a quiescent state. If your driver has any in-progress asynchronous tasks, cancel those tasks and wait for DriverKit to call the associated cancellation handler before calling the `super` version of this method.

Call `super` at the end of your implementation. After calling `super`, it’s a programmer error to access the provider object.

Don’t use this method to release your `ivars` structure; use the free method instead.

## See Also

### Running the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

free

Performs any final cleanup for the service.

