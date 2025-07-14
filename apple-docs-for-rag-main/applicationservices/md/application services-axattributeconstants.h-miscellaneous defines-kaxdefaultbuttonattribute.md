

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXDefaultButtonAttribute 

Global Variable

# kAXDefaultButtonAttribute

macOS 10.3+

``` source
var kAXDefaultButtonAttribute: String { get }
```

## Discussion

The default button of the window represented by this accessibility object. An accessibility object includes this attribute to help an assistive application easily find a window’s default button, without having to traverse the accessibility hierarchy. This attribute is recommended for all accessibility objects that represent windows that contain a default button.

