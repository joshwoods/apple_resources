

- DriverKit
- OSData
-  isEqualTo 

Instance Method

# isEqualTo

Compares the data with an OSData

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSData * aDataObj) const;
```

## Parameters 

`aDataObj`  

The OSData to compare with.

## Return Value

True iff the object is of class OSArray and isEqualTo(const OSArray \* anArray) returns true.

## Discussion

If the passed OSData object has the same length and all bytes are identical, true is returned. Otherwise false is returned.

## See Also

### Comparing Data Objects

isEqualTo

Compares the data with an OSObject

isEqualTo

Compares the data with an OSString

isEqualTo

Compares the data with a pointer to bytes

