

- NetworkingDriverKit
- IOUserNetworkEthernet
-  init 

Instance Method

# init

Handles the basic initialization of the service.

DriverKit

``` source
bool init();
```

## Return Value

`YES` if initialization was successful, or `NO` if an error occurred.

## Discussion

The system calls this method shortly after it instantiates your IOUserNetworkEthernet subclass, and before it calls the Start method of your service. Limit the work you do in this method to simple tasks that must occur before your service stats. For example, you might use this method to allocate memory for your `ivars` structure.

Always call the `super` implementation of this method at some point.

## See Also

### Configuring the Driver Service

free

Performs any final cleanup for the service.

RegisterEthernetInterface

Registers your driver with the networking stack.

