

- UIKit
- UIViewController
-  setNeedsStatusBarAppearanceUpdate() 

Instance Method

# setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+

``` source
@MainActor
func setNeedsStatusBarAppearanceUpdate()
```

## Discussion

Call this method if the view controller’s status bar attributes, such as hidden/unhidden status or style, change. If you call this method within an animation block, the changes are animated along with the rest of the animation block.

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

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

