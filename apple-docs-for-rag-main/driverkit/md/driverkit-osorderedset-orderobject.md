

- DriverKit
- OSOrderedSet
-  orderObject 

Instance Method

# orderObject

Calls the ordered set’s order function against a `NULL` object.

DriverKitiOSiPadOSmacOS

``` source
int32_t orderObject(const OSMetaClassBase * anObject);
```

## Parameters 

`anObject`  

The object to be ordered.

## Return Value

The ordering value for the object.

## Discussion

This function calls the ordered set’s order function with `anObject`, `NULL`, and the ordering context (or `NULL` if none was set), and returns the result of that function.

