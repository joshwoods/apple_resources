

- DriverKit
- OSOrderedSet
-  getLastObject 

Instance Method

# getLastObject

The last object in the ordered set if there is one, otherwise `NULL`.

DriverKitiOSiPadOSmacOS

``` source
OSObject * getLastObject() const;
```

## Discussion

The returned object will be released if removed from the ordered set; if you plan to store the reference, you should call retain on that object.

