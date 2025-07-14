

- AppKit
- NSCell
-  userInterfaceLayoutDirection 

Instance Property

# userInterfaceLayoutDirection

The layout direction of the user interface.

macOS 10.6+

``` source
@MainActor
var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

This property specifies the general user interface layout flow directions. For subclasses that have multiple visual components in a single cell instance, this property should specify the directionality or flow of components.

