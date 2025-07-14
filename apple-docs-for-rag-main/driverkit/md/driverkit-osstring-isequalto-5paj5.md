

- DriverKit
- OSString
-  isEqualTo 

Instance Method

# isEqualTo

Compares the string with an OSString.

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSString * aString) const;
```

## Parameters 

`aString`  

The OSString to compare with.

## Return Value

True iff the two strings have the same length and characters.

## Discussion

If the passed OSString object has the same length and all characters are identical, true is returned. Otherwise false is returned.

## See Also

### Comparing Strings

isEqualTo

Compares the string with an OSData.

isEqualTo

Compares the string with an OSObject

isEqualTo

Compares the string with a c-string.

