

- AppKit
- NSWindow
-  allowsToolTipsWhenApplicationIsInactive 

Instance Property

# allowsToolTipsWhenApplicationIsInactive

A Boolean value that indicates whether the window can display tooltips even when the application is in the background.

macOS

``` source
@MainActor
var allowsToolTipsWhenApplicationIsInactive: Bool { get set }
```

## Discussion

The value of this property is true if the window can display tooltips even when the application is in the background; otherwise, false. The default is false. Changing the value of this property does not take effect until the window changes to an active state.

Note

Enabling tooltips in an inactive application will cause the application to do work any time the pointer passes over the window, thus degrading system performance.

