

- DriverKit
- IOService
-  SearchProperty 

Instance Method

# SearchProperty

Searches for a property with the specified name in the current service or one of its parent services, and returns the corresponding value.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t SearchProperty(const IOPropertyName name, const IORegistryPlaneName plane, uint64_t options, OSContainer * * property);
```

## Parameters 

`name`  

The name of the property as a c-string.

`plane`  

The name of the registry plane to search. The method uses this value only when you include kIOServiceSearchPropertyParents in the `options` parameter. If you don’t include that option, you may specify `NULL` for this parameter.

`options`  

Options to use during the search. Specify kIOServiceSearchPropertyParents to expand the search to include all parent services. If you don’t specify kIOServiceSearchPropertyParents, this method looks for the property only in the current service.

`property`  

A variable in which to store the value of the property. It is a programmer error to specify `NULL` for this parameter.

If the specified property is found, this method puts the value in the provided variable; you are responsible for releasing that value. If the specified property isn’t found, this method sets the value of your variable to `NULL`.

## Return Value

kIOReturnSuccess on success, or kIOReturnNotFound if the property was not found.

## Discussion

This method searches for the property in the current service first, followed by any parent services when applicable. The method returns the first instance of the property it finds.

## See Also

### Managing the Registry Properties

CopyProperties

Returns the registry properties associated with the current service.

SetProperties

Sends the dictionary of properties to the current service object.

IOPropertyName

A string type for specifying the name of a property in the system’s registry.

IORegistryPlaneName

A string type for specifying the name of a plane in the system’s registry.

Search Options

Options to apply when searching for registry properties.

