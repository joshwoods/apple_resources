

- DriverKit
- OSOrderedSet
-  getFirstObject 

Instance Method

# getFirstObject

The object at index 0 in the ordered set if there is one, otherwise `NULL`.

DriverKitiOSiPadOSmacOS

``` source
OSObject * getFirstObject() const;
```

## Discussion

The returned object will be released if removed from the ordered set; if you plan to store the reference, you should call retain on that object.

