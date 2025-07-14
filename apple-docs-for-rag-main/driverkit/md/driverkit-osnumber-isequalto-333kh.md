

- DriverKit
- OSNumber
-  isEqualTo 

Instance Method

# isEqualTo

Compares the string with an OSObject

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSMetaClassBase * anObject) const;
```

## Parameters 

`anObject`  

The object to compare with.

## Return Value

True iff the object is of class OSNumber isEqualTo() returns true.

## Discussion

If the object is of class OSNumber, the result of isEqualTo(const OSNumber \* aDataObj) is returned. Otherwise false is returned.

## See Also

### Comparing Numbers

isEqualTo

Compares the number with an OSNumber.

