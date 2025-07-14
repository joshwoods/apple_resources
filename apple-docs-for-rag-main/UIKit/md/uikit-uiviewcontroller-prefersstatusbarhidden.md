

- UIKit
- UIViewController
-  prefersStatusBarHidden 

Instance Property

# prefersStatusBarHidden

Specifies whether the view controller prefers the status bar to be hidden or shown.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0–1.0Deprecated

``` source
@MainActor
var prefersStatusBarHidden: Bool { get }
```

## Return Value

true if the status bar should be hidden or false if it should be shown.

## Discussion

If you change the return value for this method, call the setNeedsStatusBarAppearanceUpdate() method. To specify that a child view controller should control preferred status bar hidden/unhidden state, implement the childForStatusBarHidden method.

By default, this method returns false with one exception. For apps linked against iOS 8 or later, this method returns true if the view controller is in a vertically compact environment.

## See Also

### Managing the status bar

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

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

