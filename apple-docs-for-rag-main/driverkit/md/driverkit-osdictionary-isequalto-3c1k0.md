

- DriverKit
- OSDictionary
-  isEqualTo 

Instance Method

# isEqualTo

Compares all members of two dictionaries with isEqualTo().

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSDictionary * aDictionary) const;
```

## Parameters 

`aDictionary`  

The other dictionary to compare with.

## Return Value

True if both dictionaries have equal counts, every key exists in both, values for each key compare true with isEqualTo().

## Discussion

If the dictionaries have equal counts, each member is compared with the other at the same index with isEqualTo(). Otherwise false is returned.

## See Also

### Comparing Dictionaries

isEqualTo

Compares certain members of two dictionaries with isEqualTo().

isEqualTo

Compares the dictionary with an OSObject

