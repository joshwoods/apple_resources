

- UIKit
- UIViewController
-  childForStatusBarStyle 

Instance Property

# childForStatusBarStyle

Called when the system needs the view controller to use for determining status bar style.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0–1.0Deprecated

``` source
@MainActor
var childForStatusBarStyle: UIViewController? { get }
```

## Return Value

The view controller whose status bar style should be used.

## Discussion

If your container view controller derives its status bar style from one of its child view controllers, implement this method and return that child view controller. If you return `nil` or do not override this method, the status bar style for `self` is used. If the return value from this method changes, call the setNeedsStatusBarAppearanceUpdate() method.

## See Also

### Managing the status bar

var prefersStatusBarHidden: Bool

Specifies whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarHidden: UIViewController?

The view controller to use for determining the hidden state of the status bar.

var preferredStatusBarStyle: UIStatusBarStyle

The preferred status bar style for the view controller.

enum UIStatusBarStyle

Constants that describe the style of the device’s status bar.

var modalPresentationCapturesStatusBarAppearance: Bool

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

