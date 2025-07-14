

- DriverKit
- OSMetaClassBase
-  isEqualTo 

Instance Method

# isEqualTo

Compares two objects

DriverKitiOSiPadOSmacOS

``` source
bool isEqualTo(const OSMetaClassBase * anObject) const;
```

## Discussion

The default implementation only compares the object pointers, however many container classes override to provide deeper comparison.

