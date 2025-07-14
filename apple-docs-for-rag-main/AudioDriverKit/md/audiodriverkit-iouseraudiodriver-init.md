

- AudioDriverKit
- IOUserAudioDriver
-  init 

Instance Method

# init

Handles the basic initialization of the service.

DriverKit 21.0+

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## Discussion

Override this method inherited from IOService.

The system calls this method shortly after it instantiates your custom IOService subclass, and before it calls the Start method of your service. Limit the work you do in this method to simple tasks that must occur before your service starts. For example, use this method to allocate memory for your `ivars` structure.

Always call `super` early in your implementation of this method.

## See Also

### Running the Driver Service

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

