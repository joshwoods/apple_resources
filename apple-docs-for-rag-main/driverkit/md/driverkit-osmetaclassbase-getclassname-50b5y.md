

- DriverKit
- OSMetaClassBase
-  GetClassName 

Instance Method

# GetClassName

Returns the name of the class given an OSObject pointer.

DriverKitiOSiPadOSmacOS

``` source
const char * GetClassName();
```

## Return Value

C-string class name, valid while the object is retained.

## See Also

### Getting Meta Information

IsRemote

GetClass

Internal helper for GetClassName. Not to be called directly.

getMetaClass

Internal helper for GetClassName. Not to be called directly.

