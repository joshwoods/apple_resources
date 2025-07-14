

- AudioDriverKit
- IOUserAudioDriver
-  free 

Instance Method

# free

Performs any final cleanup for the service.

DriverKit 21.0+

``` source
void free();
```

## Discussion

Override this method inherited from IOService.

Use this method to perform any final cleanup of your service, such as deallocating any memory you allocated. The system calls this method at some point after it calls your service’s Stop method.

Always call `super` at the end of your custom implementation.

## See Also

### Running the Driver Service

init

Handles the basic initialization of the service.

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

