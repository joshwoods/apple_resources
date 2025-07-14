

- DriverKit
- OSSet
-  member 

Instance Method

# member

Checks the set for the presence of an object.

DriverKitiOSiPadOSmacOS

``` source
bool member(const OSMetaClassBase * anObject) const;
```

## Parameters 

`anObject`  

The OSMetaClassBase-derived object to check for in the set.

## Return Value

`true` if `anObject` is present within the set, `false` otherwise.

## Discussion

Pointer equality is used. This function returns `false` if passed `NULL`.

containsObject checks for `NULL` first, and is therefore more efficient than this function.

