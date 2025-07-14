

- UIKit
- UIViewController
-  preferredStatusBarUpdateAnimation 

Instance Property

# preferredStatusBarUpdateAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0–1.0Deprecated

``` source
@MainActor
var preferredStatusBarUpdateAnimation: UIStatusBarAnimation { get }
```

## Return Value

The style of status bar animation to use; one of the constants from the UIStatusBarAnimation enum. Default value is UIStatusBarAnimation.fade.

## Discussion

This property comes into play only when you actively change the status bar’s show/hide state by changing the return value of the prefersStatusBarHidden method.

## See Also

### Managing the status bar

var prefersStatusBarHidden: Bool

Specifies whether the view controller prefers the status bar to be hidden or shown.

var childForStatusBarHidden: UIViewController?

The view controller to use for determining the hidden state of the status bar.

var childForStatusBarStyle: UIViewController?

Called when the system needs the view controller to use for determining status bar style.

var preferredStatusBarStyle: UIStatusBarStyle

The preferred status bar style for the view controller.

enum UIStatusBarStyle

Constants that describe the style of the device’s status bar.

var modalPresentationCapturesStatusBarAppearance: Bool

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

