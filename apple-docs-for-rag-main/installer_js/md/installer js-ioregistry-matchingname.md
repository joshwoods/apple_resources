

- Installer JS
- IORegistry
-  matchingName 

# matchingName

Returns the IOKit objects of the specified name.

``` source
matchingName(objectName, [servicePlane])
```

## Parameters 

`objectName`  

String with an IOKit object name.

`servicePlane`  

*Optional*. String with the service plane to search. When unspecified, `'IOServicePlane'` is used.

## Return Value

An array of IOKit object dictionaries.

## See Also

### Accessing the IOKit Registry

fromPath

Returns a dictionary with the properties of a given IOKit object.

matchingClass

Returns the IOKit objects of a given class.

childrenOf

Returns the children of the given IOKit object.

parentsOf

Returns the parents of the given IOKit object.

