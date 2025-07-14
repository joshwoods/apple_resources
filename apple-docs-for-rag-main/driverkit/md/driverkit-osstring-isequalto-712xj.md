

- DriverKit
- OSString
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

True iff the object is of class OSData or OSString and isEqualTo() returns true.

## Discussion

If the object is of class OSString, the result of isEqualTo(const OSString \* aDataObj) is returned. If the object is of class OSData, the result of isEqualTo(const OSData \* aDataObj) is returned. Otherwise false is returned.

## See Also

### Comparing Strings

isEqualTo

Compares the string with an OSData.

isEqualTo

Compares the string with an OSString.

isEqualTo

Compares the string with a c-string.

