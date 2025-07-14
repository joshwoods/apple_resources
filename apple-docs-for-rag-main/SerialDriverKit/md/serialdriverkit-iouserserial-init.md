

- SerialDriverKit
- IOUserSerial
-  init 

Instance Method

# init

Handles the basic initialization of the service.

DriverKit 19.0+

``` source
bool init();
```

## Return Value

`YES` if initialization is successful, or `NO` if an error occurred.

## Discussion

The system calls this method shortly after it instantiates your `IOUserSerial` subclass, and before it calls the Start method of your service. Override this method and use it to initialize your subclass. Limit the work you do in this method to simple tasks that must occur before your service starts. For example, use this method to allocate memory for your `ivars` structure.

Always call `super` at the beginning of your implementation of this method.

## See Also

### Configuring the Service

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

initWith

Initializes the private data structures associated with this class.

