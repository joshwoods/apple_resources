

- BlockStorageDeviceDriverKit
- IOUserBlockStorageDevice
-  free 

Instance Method

# free

Performs any final cleanup for the service.

DriverKit 21.0+

``` source
void free();
```

## Discussion

Use this method to perform tasks such as deallocating any allocated memory. The system calls this method at some point after it calls your service’s Stop method.

Always call `super` at the end of your custom implementation.

## See Also

### Running the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

