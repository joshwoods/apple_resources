

- UIKit
- UIViewController
-  preferredStatusBarStyle 

Instance Property

# preferredStatusBarStyle

The preferred status bar style for the view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0–1.0Deprecated

``` source
@MainActor
var preferredStatusBarStyle: UIStatusBarStyle { get }
```

## Return Value

A UIStatusBarStyle key indicating your preferred status bar style for the view controller.

## Discussion

You can override the preferred status bar style for a view controller by implementing the childForStatusBarStyle method.

If the return value from this method changes, call the setNeedsStatusBarAppearanceUpdate() method.

## See Also

### Managing the status bar

var prefersStatusBarHidden: Bool

Specifies whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarHidden: UIViewController?

The view controller to use for determining the hidden state of the status bar.

var childForStatusBarStyle: UIViewController?

Called when the system needs the view controller to use for determining status bar style.

enum UIStatusBarStyle

Constants that describe the style of the device’s status bar.

var modalPresentationCapturesStatusBarAppearance: Bool

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

