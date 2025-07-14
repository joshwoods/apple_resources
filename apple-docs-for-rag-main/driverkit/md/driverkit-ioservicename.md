

- DriverKit
-  IOServiceName 

Type Alias

# IOServiceName

A string type for setting the name of the service in the system’s registry.

DriverKitiOSiPadOSmacOS

``` source
typedef char[128] IOServiceName;
```

## See Also

### Registering the Service with IOKit

RegisterService

Starts the registration process for the service and performs any additional matching.

SetName

Sets the name of the service in the system’s registry.

GetRegistryEntryID

Returns the registry ID for the current service.

