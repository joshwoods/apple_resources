

- DriverKit
- OSArray
-  isEqualTo 

Instance Method

# isEqualTo

Compares all members of two arrays with isEqualTo().

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSArray * anArray) const;
```

## Parameters 

`anArray`  

The other array to compare with.

## Return Value

True if both arrays have equal counts and all members compare successfully with isEqualTo.

## Discussion

If the arrays have equal counts, each member is compared with the other at the same index with isEqualTo(). Otherwise false is returned.

## See Also

### Comparing Arrays

isEqualTo

Compares the array with an OSObject

