

- AppKit
- NSOutlineView
-  userInterfaceLayoutDirection 

Instance Property

# userInterfaceLayoutDirection

The user interface layout direction.

macOS 10.7+

``` source
@MainActor
var userInterfaceLayoutDirection: NSUserInterfaceLayoutDirection { get set }
```

## Discussion

When set to NSUserInterfaceLayoutDirection.rightToLeft, the outline view displays the disclosure triangle to the right of the cell instead of the left. The default value is NSUserInterfaceLayoutDirection.leftToRight.

