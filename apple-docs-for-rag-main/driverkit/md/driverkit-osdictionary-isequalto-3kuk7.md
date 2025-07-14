

- DriverKit
- OSDictionary
-  isEqualTo 

Instance Method

# isEqualTo

Compares the dictionary with an OSObject

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSMetaClassBase * anObject) const;
```

## Parameters 

`anObject`  

The object to compare with.

## Return Value

True iff the object is of class OSDictionary and isEqualTo(const OSDictionary \* anArray) returns true.

## Discussion

If the object is of class OSDictionary, the result of isEqualTo(const OSDictionary \* anArray) is returned. Otherwise false is returned.

## See Also

### Comparing Dictionaries

isEqualTo

Compares all members of two dictionaries with isEqualTo().

isEqualTo

Compares certain members of two dictionaries with isEqualTo().

