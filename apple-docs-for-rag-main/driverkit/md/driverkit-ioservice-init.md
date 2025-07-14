

- DriverKit
- IOService
-  init 

Instance Method

# init

Handles the basic initialization of the service.

DriverKitiOSiPadOSmacOS

``` source
bool init();
```

## Return Value

`true` if initialization was successful, or `false` if an error occurred.

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Discussion

The system calls this method shortly after it instantiates your custom IOService subclass, and before it calls the Start method of your service. Limit the work you do in this method to simple tasks that must occur before your service starts. For example, use this method to allocate memory for your `ivars` structure.

Always call `super` early in your implementation of this method.

## See Also

### Running the Service

Start

Starts the current service and associates it with the specified provider.

Stop

Stops the service associated with the specified provider.

free

Performs any final cleanup for the service.

