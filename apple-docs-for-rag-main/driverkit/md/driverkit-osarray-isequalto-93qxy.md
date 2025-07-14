

- DriverKit
- OSArray
-  isEqualTo 

Instance Method

# isEqualTo

Compares the array with an OSObject

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSMetaClassBase * anObject) const;
```

## Parameters 

`anObject`  

The object to compare with.

## Return Value

True iff the object is of class OSArray and isEqualTo(const OSArray \* anArray) returns true.

## Discussion

If the object is of class OSArray, the result of isEqualTo(const OSArray \* anArray) is returned. Otherwise false is returned.

## See Also

### Comparing Arrays

isEqualTo

Compares all members of two arrays with isEqualTo().

