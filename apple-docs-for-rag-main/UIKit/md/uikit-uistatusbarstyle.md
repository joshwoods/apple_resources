

- UIKit
-  UIStatusBarStyle 

Enumeration

# UIStatusBarStyle

Constants that describe the style of the device’s status bar.

iOSiPadOSMac CatalystvisionOS

``` source
enum UIStatusBarStyle
```

## Topics

### Constants

case `default`

A style that automatically selects an appearance for the status bar and updates it dynamically to maintain contrast with the content below it.

case lightContent

A light status bar, intended for use on dark backgrounds.

case darkContent

A dark status bar, intended for use on light backgrounds.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var modalPresentationCapturesStatusBarAppearance: Bool

Specifies whether a view controller, presented non-fullscreen, takes over control of status bar appearance from the presenting view controller.

var preferredStatusBarUpdateAnimation: UIStatusBarAnimation

Specifies the animation style to use for hiding and showing the status bar for the view controller.

func setNeedsStatusBarAppearanceUpdate()

Indicates to the system that the view controller status bar attributes have changed.

