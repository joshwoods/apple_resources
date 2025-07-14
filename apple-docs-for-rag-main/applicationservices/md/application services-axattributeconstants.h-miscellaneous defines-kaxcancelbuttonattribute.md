

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXCancelButtonAttribute 

Global Variable

# kAXCancelButtonAttribute

macOS 10.3+

``` source
var kAXCancelButtonAttribute: String { get }
```

## Discussion

The cancel button of the window represented by this accessibility object. An accessibility object includes this attribute to help an assistive application easily find a window’s cancel button, without having to traverse the accessibility hierarchy. This attribute is recommended for all accessibility objects that represent windows that contain a cancel button.

