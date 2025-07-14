

- DriverKit
- IOService
-  RegisterService 

Instance Method

# RegisterService

Starts the registration process for the service and performs any additional matching.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t RegisterService();
```

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Mentioned in 

Creating a Driver Using the DriverKit SDK

## Discussion

After setting up your service in your custom Start method, call this method to let the system know your service is running.

## See Also

### Registering the Service with IOKit

SetName

Sets the name of the service in the system’s registry.

GetRegistryEntryID

Returns the registry ID for the current service.

IOServiceName

A string type for setting the name of the service in the system’s registry.

