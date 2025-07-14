

- DriverKit
- OSData
-  isEqualTo 

Instance Method

# isEqualTo

Compares the data with an OSObject

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSMetaClassBase * anObject) const;
```

## Parameters 

`anObject`  

The object to compare with.

## Return Value

True iff the object is of class OSData or OSString and isEqualTo() returns true.

## Discussion

If the object is of class OSData, the result of isEqualTo(const OSData \* aDataObj) is returned. If the object is of class OSString, the result of OSString::isEqualTo(const OSData \* aDataObj) is returned. Otherwise false is returned.

## See Also

### Comparing Data Objects

isEqualTo

Compares the data with an OSData

isEqualTo

Compares the data with an OSString

isEqualTo

Compares the data with a pointer to bytes

