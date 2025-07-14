

- DriverKit
- IOService
-  SetName 

Instance Method

# SetName

Sets the name of the service in the system’s registry.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetName(const IOServiceName name);
```

## Parameters 

`name`  

The new name for the service. This method copies the string you provide.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Registering the Service with IOKit

RegisterService

Starts the registration process for the service and performs any additional matching.

GetRegistryEntryID

Returns the registry ID for the current service.

IOServiceName

A string type for setting the name of the service in the system’s registry.

