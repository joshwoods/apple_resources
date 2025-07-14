

- DriverKit
-  IODelete 

Macro

# IODelete

Frees the memory associated with a valid, typed array.

DriverKitiOSiPadOSmacOS

``` source
#define IODelete(ptr, type, count)
```

## Parameters 

`ptr`  

The pointer to the memory block to free. This pointer must not be `NULL`.

`type`  

The data type stored in the memory block. The macro uses the type to determine its size.

`count`  

The number of array entries in the memory block

## Discussion

Use this macro to free memory that you allocated with IONew or IONewZero. It is a programmer error to pass a `NULL` pointer to this macro.

## See Also

### Deallocation

IOSafeDeleteNULL

Frees the memory associated with a typed array.

OSSafeReleaseNULL

Frees memory that you allocated for a named class.

IOFree

Frees a memory block that contains general-purpose memory.

