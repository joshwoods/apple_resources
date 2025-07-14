

- UIKit
- UIWindow
-  windowLevel 

Instance Property

# windowLevel

The position of the window in the z-axis.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var windowLevel: UIWindow.Level { get set }
```

## Discussion

Window levels provide a relative grouping of windows along the z-axis. All windows assigned to the same window level appear in front of (or behind) all windows assigned to a different window level. The ordering of windows within a given window level is not guaranteed.

The default value of this property is normal. For a list of other possible window levels, see UIWindow.Level.

## See Also

### Configuring the window

var rootViewController: UIViewController?

The root view controller for the window.

struct Level

The positioning of windows relative to each other.

var canResizeToFitContent: Bool

A Boolean value that indicates whether the window’s constraint-based content determines its size.

var screen: UIScreen

The screen to display the window on.

Deprecated

