

- DriverKit
-  IOPropertyName 

Type Alias

# IOPropertyName

A string type for specifying the name of a property in the system’s registry.

DriverKitiOSiPadOSmacOS

``` source
typedef char[128] IOPropertyName;
```

## See Also

### Managing the Registry Properties

CopyProperties

Returns the registry properties associated with the current service.

SetProperties

Sends the dictionary of properties to the current service object.

SearchProperty

Searches for a property with the specified name in the current service or one of its parent services, and returns the corresponding value.

IORegistryPlaneName

A string type for specifying the name of a plane in the system’s registry.

Search Options

Options to apply when searching for registry properties.

