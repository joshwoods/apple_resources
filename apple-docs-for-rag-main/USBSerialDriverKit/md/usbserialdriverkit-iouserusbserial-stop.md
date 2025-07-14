

- USBSerialDriverKit
- IOUserUSBSerial
-  Stop 

Instance Method

# Stop

Stops the service that matches the specified provider.

DriverKit 19.0+

``` source
kern_return_t Stop(IOService * provider);
```

## Parameters 

`provider`  

The provider associated with the current service. This object is the same one that the system previously passed to your service’s Start method.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. See Error Codes.

## Discussion

Before terminating a provider, the system calls this method to stop the service associated with that object. Use your implementation of this method to stop all activity and put your driver in a quiescent state. Call `super` at the end of your implementation. After you call `super`, it is a programmer error to access the `provider` object.

## See Also

### Configuring the Service

init

Handles the basic initialization of the service.

Start

Starts the service for the specified provider.

free

Performs any final cleanup for the service.

initWith

Initializes the private data structures associated with this class.

