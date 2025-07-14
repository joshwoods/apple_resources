

- DriverKit
- IOService
-  SetProperties 

Instance Method

# SetProperties

Sends the dictionary of properties to the current service object.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SetProperties(OSDictionary * properties);
```

## Parameters 

`properties`  

The registry properties to associate with the current service.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

The default implementation of this method returns kIOReturnUnsupported. You can override this method and use it to modify the set of properties and values as needed. The changes you make apply only to the current service.

## See Also

### Managing the Registry Properties

CopyProperties

Returns the registry properties associated with the current service.

SearchProperty

Searches for a property with the specified name in the current service or one of its parent services, and returns the corresponding value.

IOPropertyName

A string type for specifying the name of a property in the system’s registry.

IORegistryPlaneName

A string type for specifying the name of a plane in the system’s registry.

Search Options

Options to apply when searching for registry properties.

