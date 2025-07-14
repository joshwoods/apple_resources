

- AppKit
- NSWindow
-  isExcludedFromWindowsMenu 

Instance Property

# isExcludedFromWindowsMenu

A Boolean value that indicates whether the window is excluded from the application’s Windows menu.

macOS

``` source
@MainActor
var isExcludedFromWindowsMenu: Bool { get set }
```

## Discussion

The value of this property is true when the window is excluded from the Windows menu; otherwise, false. The default initial setting is false.

