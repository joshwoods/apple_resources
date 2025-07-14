

- NetworkingDriverKit
- IOUserNetworkEthernet
-  free 

Instance Method

# free

Performs any final cleanup for the service.

DriverKit

``` source
void free();
```

## Discussion

Use this method to perform any final cleanup of your service, such as deallocating any memory associated with your service. The system calls this method at some point after it calls your service’s Stop method.

## See Also

### Configuring the Driver Service

init

Handles the basic initialization of the service.

RegisterEthernetInterface

Registers your driver with the networking stack.

