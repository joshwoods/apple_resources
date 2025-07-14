

- SerialDriverKit
- IOUserSerial
-  free 

Instance Method

# free

Performs any final cleanup for the service.

DriverKit 19.0+

``` source
void free();
```

## Discussion

Use this method to deallocate the memory associated with your service, or perform other cleanup tasks. The system calls this method at some point after it calls your service’s Stop method.

Always call `super` at the end of your implementation of this method.

## See Also

### Configuring the Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

initWith

Initializes the private data structures associated with this class.

