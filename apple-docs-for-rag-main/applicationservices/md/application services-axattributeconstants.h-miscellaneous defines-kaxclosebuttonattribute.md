

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXCloseButtonAttribute 

Global Variable

# kAXCloseButtonAttribute

macOS 10.2+

``` source
var kAXCloseButtonAttribute: String { get }
```

## Discussion

The close button of the window represented by this accessibility object. An accessibility object includes this attribute to help an assistive application easily find a window’s close button, without having to traverse the accessibility hierarchy. This attribute is recommended for all accessibility objects that represent windows that contain a close button.

