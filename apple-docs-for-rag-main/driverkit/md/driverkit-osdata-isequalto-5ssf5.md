

- DriverKit
- OSData
-  isEqualTo 

Instance Method

# isEqualTo

Compares the data with an OSString

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSString * aString) const;
```

## Parameters 

`aString`  

The object to compare with.

## Return Value

True if the OSData and OSString contain the same c-string.

## Discussion

If the passed OSString object has the same length and all bytes are identical, true is returned. If the passed OSString object has a length one byte less than the OSData, all bytes are identical, and the last byte of the OSData is zero, true is returned. Otherwise false is returned.

## See Also

### Comparing Data Objects

isEqualTo

Compares the data with an OSData

isEqualTo

Compares the data with an OSObject

isEqualTo

Compares the data with a pointer to bytes

