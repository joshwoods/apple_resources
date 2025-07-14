

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXFocusedAttribute 

Global Variable

# kAXFocusedAttribute

macOS 10.2+

``` source
var kAXFocusedAttribute: String { get }
```

## Discussion

Indicates whether the accessibility object currently has the keyboard focus. Note that you can set the value of the `AXFocused` attribute to `true` to accept keyboard focus. This attribute is required for all accessibility objects representing elements that can receive keyboard focus.

