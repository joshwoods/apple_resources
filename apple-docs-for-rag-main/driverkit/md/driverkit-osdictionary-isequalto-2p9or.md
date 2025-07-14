

- DriverKit
- OSDictionary
-  isEqualTo 

Instance Method

# isEqualTo

Compares certain members of two dictionaries with isEqualTo().

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSDictionary * aDictionary, const OSCollection * keys) const;
```

## Parameters 

`aDictionary`  

The other dictionary to compare with.

`keys`  

The collection of keys to compare.

## Return Value

True if both dictionaries have equal counts, every key exists in both, values for each key compare true with isEqualTo().

## Discussion

For each key in the given collection, both dictionaries must contain values for the key that compare successfully with isEqualTo().

## See Also

### Comparing Dictionaries

isEqualTo

Compares all members of two dictionaries with isEqualTo().

isEqualTo

Compares the dictionary with an OSObject

