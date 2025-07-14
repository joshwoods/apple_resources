

- AppKit
- NSMenuItem
-  isEnabled 

Instance Property

# isEnabled

A Boolean value that indicates whether the menu item is enabled.

macOS

``` source
var isEnabled: Bool { get set }
```

## Discussion

This property has no effect unless the menu in which the item will be added or is already a part of has been sent `setAutoenablesItems:NO`. If a menu item is disabled, its keyboard equivalent is also disabled. See the `NSMenuValidation` informal protocol specification for cautions regarding this method.

