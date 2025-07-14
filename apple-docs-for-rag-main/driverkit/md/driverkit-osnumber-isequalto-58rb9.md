

- DriverKit
- OSNumber
-  isEqualTo 

Instance Method

# isEqualTo

Compares the number with an OSNumber.

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSNumber * aNumber) const;
```

## Parameters 

`aNumber`  

The OSNumber to compare with.

## Return Value

True iff the two numbers have the same value.

## Discussion

If the passed OSNumber object has the same value, regardless of size, true is returned. Otherwise false is returned.

## See Also

### Comparing Numbers

isEqualTo

Compares the string with an OSObject

