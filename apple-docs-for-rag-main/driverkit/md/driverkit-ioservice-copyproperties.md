

- DriverKit
- IOService
-  CopyProperties 

Instance Method

# CopyProperties

Returns the registry properties associated with the current service.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t CopyProperties(OSDictionary * * properties);
```

## Parameters 

`properties`  

A variable for storing the properties. On return, the variable contains a dictionary with the properties, or `NULL` if the service has no registered properties. If this method returns a valid dictionary, you are responsible for releasing that dictionary when you are finished with it.

It is a programmer error to specify `NULL` or an invalid pointer for this parameter.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## See Also

### Managing the Registry Properties

SetProperties

Sends the dictionary of properties to the current service object.

SearchProperty

Searches for a property with the specified name in the current service or one of its parent services, and returns the corresponding value.

IOPropertyName

A string type for specifying the name of a property in the system’s registry.

IORegistryPlaneName

A string type for specifying the name of a plane in the system’s registry.

Search Options

Options to apply when searching for registry properties.

