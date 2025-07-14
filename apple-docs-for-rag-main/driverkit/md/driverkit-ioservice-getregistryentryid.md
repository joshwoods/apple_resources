

- DriverKit
- IOService
-  GetRegistryEntryID 

Instance Method

# GetRegistryEntryID

Returns the registry ID for the current service.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t GetRegistryEntryID(uint64_t * registryEntryID);
```

## Parameters 

`registryEntryID`  

A pointer to an integer that, on return, contains the registry ID for the service. It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Registering the Service with IOKit

RegisterService

Starts the registration process for the service and performs any additional matching.

SetName

Sets the name of the service in the system’s registry.

IOServiceName

A string type for setting the name of the service in the system’s registry.

