

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXMainAttribute 

Global Variable

# kAXMainAttribute

macOS 10.2+

``` source
var kAXMainAttribute: String { get }
```

## Discussion

Indicates whether the window represented by this accessibility object is the main application window. Note that a window can be main even though it does not have keyboard focus. This attribute is recommended for all accessibility objects that represent windows.

