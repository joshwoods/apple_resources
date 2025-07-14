

- UIKit
- UIViewController
-  modalPresentationCapturesStatusBarAppearance 

Instance Property

# modalPresentationCapturesStatusBarAppearance

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var modalPresentationCapturesStatusBarAppearance: Bool { get set }
```

## Discussion

The default value of this property is false.

When you present a view controller by calling the present(_:animated:completion:) method, status bar appearance control is transferred from the presenting to the presented view controller only if the presented controller’s modalPresentationStyle value is UIModalPresentationStyle.fullScreen. By setting this property to true, you specify the presented view controller controls status bar appearance, even though presented non-fullscreen.

The system ignores this property’s value for a view controller presented fullscreen.

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

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

