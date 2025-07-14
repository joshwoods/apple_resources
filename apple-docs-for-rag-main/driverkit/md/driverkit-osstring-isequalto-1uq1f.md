

- DriverKit
- OSString
-  isEqualTo 

Instance Method

# isEqualTo

Compares the string with an OSData.

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSData * aDataObject) const;
```

## Parameters 

`aDataObject`  

The OSData to compare with.

## Return Value

True if the OSData and OSString contain the same c-string.

## Discussion

If the passed OSData object has the same length and all bytes are identical, true is returned. If the passed OSData object has a length one byte greater than the OSString, all bytes are identical, and the last byte of the OSData is zero, true is returned. Otherwise false is returned.

## See Also

### Comparing Strings

isEqualTo

Compares the string with an OSObject

isEqualTo

Compares the string with an OSString.

isEqualTo

Compares the string with a c-string.

