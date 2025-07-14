

- DriverKit
- OSString
-  isEqualTo 

Instance Method

# isEqualTo

Compares the string with a c-string.

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const char * cString) const;
```

## Parameters 

`cString`  

The c-string to compare with.

## Return Value

True iff the two strings have the same length and characters.

## Discussion

If the passed c-string has the same length and all characters are identical to those in the OSString, true is returned. Otherwise false is returned.

## See Also

### Comparing Strings

isEqualTo

Compares the string with an OSData.

isEqualTo

Compares the string with an OSObject

isEqualTo

Compares the string with an OSString.

