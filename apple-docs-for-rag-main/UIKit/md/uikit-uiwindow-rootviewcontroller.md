

- UIKit
- UIWindow
-  rootViewController 

Instance Property

# rootViewController

The root view controller for the window.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var rootViewController: UIViewController? { get set }
```

## Mentioned in 

Managing content in your app’s windows

## Discussion

The root view controller provides the content view of the window. Assigning a view controller to this property (either programmatically or using Interface Builder) installs the view controller’s view as the content view of the window. The new content view is configured to track the window size, changing as the window size changes. If the window has an existing view hierarchy, the old views are removed before the new ones are installed.

The default value of this property is `nil`.

## See Also

### Configuring the window

var windowLevel: UIWindow.Level

The position of the window in the z-axis.

struct Level

The positioning of windows relative to each other.

var canResizeToFitContent: Bool

A Boolean value that indicates whether the window’s constraint-based content determines its size.

var screen: UIScreen

The screen to display the window on.

Deprecated

