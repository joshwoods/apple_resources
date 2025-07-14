

- UIKit
- UIViewController
-  childForStatusBarHidden 

Instance Property

# childForStatusBarHidden

The view controller to use for determining the hidden state of the status bar.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0–1.0Deprecated

``` source
@MainActor
var childForStatusBarHidden: UIViewController? { get }
```

## Discussion

If your container view controller derives the hidden state of the status bar from one of its child view controllers, implement this property to specify which child view controller you want to control the hidden/unhidden state. If you return `nil` or don’t override this property, the status bar hidden/unhidden state for `self` is used.

Call setNeedsStatusBarAppearanceUpdate() if the child view controller for determining the hidden state of the status bar changes.

## See Also

### Managing the status bar

var prefersStatusBarHidden: Bool

Specifies whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarStyle: UIViewController?

Called when the system needs the view controller to use for determining status bar style.

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

