

- Application Services
- AXAttributeConstants.h
- Miscellaneous Defines
-  kAXEnabledAttribute 

Global Variable

# kAXEnabledAttribute

macOS 10.2+

``` source
var kAXEnabledAttribute: String { get }
```

## Discussion

Indicates whether the user can interact with the accessibility object. For example, the `AXEnabled` attribute of a disabled button is `false`. This attribute is required for accessibility objects that represent views, menus, and menu items. This attribute is not required for accessibility objects that represent windows.

