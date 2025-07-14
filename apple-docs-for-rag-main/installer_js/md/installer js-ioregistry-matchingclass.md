

- Installer JS
- IORegistry
-  matchingClass 

# matchingClass

Returns the IOKit objects of a given class.

``` source
matchingClass(className, [servicePlane])
```

## Parameters 

`className`  

String with an IOKit class name.

`servicePlane`  

*Optional*. String with the service plane to search. When unspecified, `'IOServicePlane'` is used.

## Return Value

An array of IOKit object dictionaries.

## See Also

### Accessing the IOKit Registry

fromPath

Returns a dictionary with the properties of a given IOKit object.

matchingName

Returns the IOKit objects of the specified name.

childrenOf

Returns the children of the given IOKit object.

parentsOf

Returns the parents of the given IOKit object.

