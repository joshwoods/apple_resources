

- Application Services
- Carbon Accessibility
- Attributes
-  kAXMenuItemCmdVirtualKeyAttribute 

Global Variable

# kAXMenuItemCmdVirtualKeyAttribute

macOS 10.2+

``` source
var kAXMenuItemCmdVirtualKeyAttribute: String { get }
```

## Discussion

The key code associated with the physical key in the keyboard shortcut for the command represented by this accessibility object. For example, Return and Enter are different physical keys that can produce the same character. If an assistive application needs to be able to distinguish between them, it can view the virtual key codes.

