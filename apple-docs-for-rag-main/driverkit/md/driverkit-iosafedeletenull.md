

- DriverKit
-  IOSafeDeleteNULL 

Macro

# IOSafeDeleteNULL

Frees the memory associated with a typed array.

DriverKitiOSiPadOSmacOS

``` source
#define IOSafeDeleteNULL(ptr, type, count)
```

## Parameters 

`ptr`  

The pointer to the memory block to free. You may specify `NULL` for this parameter. After freeing the memory, the macro sets the value of `ptr` to `NULL`.

`type`  

The data type stored in the memory block. The macro uses the type to determine its size.

`count`  

The number of array entries in the memory block

## Discussion

Use this macro to free memory that you allocated with IONew or IONewZero. If `ptr` is `NULL`, this macro doesn’t attempt to free the memory.

## See Also

### Deallocation

IODelete

Frees the memory associated with a valid, typed array.

OSSafeReleaseNULL

Frees memory that you allocated for a named class.

IOFree

Frees a memory block that contains general-purpose memory.

