

- DriverKit
- OSData
-  isEqualTo 

Instance Method

# isEqualTo

Compares the data with a pointer to bytes

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const void * bytes, size_t numBytes) const;
```

## Parameters 

`bytes`  

C-pointer to untyped data.

`numBytes`  

Count of bytes to be compared.

## Return Value

True iff the length of the data are equal and all bytes are identical.

## Discussion

If the passed data has the same length and all bytes are identical, true is returned. Otherwise false is returned.

## See Also

### Comparing Data Objects

isEqualTo

Compares the data with an OSData

isEqualTo

Compares the data with an OSObject

isEqualTo

Compares the data with an OSString

