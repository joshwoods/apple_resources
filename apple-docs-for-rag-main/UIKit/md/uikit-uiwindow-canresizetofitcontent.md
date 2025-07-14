

- UIKit
- UIWindow
-  canResizeToFitContent 

Instance Property

# canResizeToFitContent

A Boolean value that indicates whether the window’s constraint-based content determines its size.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOSvisionOS 1.0+

``` source
@MainActor
var canResizeToFitContent: Bool { get set }
```

## Discussion

The default value of this property is false, which causes the window to maintain a fixed size. Setting this property to true allows the system to perform constraints-based window sizing, which updates the window’s size to match the space needed by its content. Window-size changes occur only when the app runs on macOS.

## See Also

### Configuring the window

var rootViewController: UIViewController?

The root view controller for the window.

var windowLevel: UIWindow.Level

The position of the window in the z-axis.

struct Level

The positioning of windows relative to each other.

var screen: UIScreen

The screen to display the window on.

Deprecated

