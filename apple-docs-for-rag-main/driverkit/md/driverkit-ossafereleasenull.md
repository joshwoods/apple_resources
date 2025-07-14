

- DriverKit
-  OSSafeReleaseNULL 

Macro

# OSSafeReleaseNULL

Frees memory that you allocated for a named class.

DriverKitiOSiPadOSmacOS

``` source
#define OSSafeReleaseNULL(inst)
```

## Parameters 

`inst`  

The object that you want to free. After freeing the memory, the macro sets the value of `inst` to `NULL`.

## Discussion

Use this macro to free memory that you allocated OSTypeAlloc. If `inst` is `NULL`, this macro doesn’t attempt to free the memory.

## See Also

### Deallocation

IODelete

Frees the memory associated with a valid, typed array.

IOSafeDeleteNULL

Frees the memory associated with a typed array.

IOFree

Frees a memory block that contains general-purpose memory.

