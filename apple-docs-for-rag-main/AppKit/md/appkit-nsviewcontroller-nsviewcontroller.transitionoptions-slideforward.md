

- AppKit
- NSViewController
- NSViewController.TransitionOptions
-  slideForward 

Type Property

# slideForward

A transition animation that reflects the user interface layout direction (userInterfaceLayoutDirection) in a “forward” manner, as follows:

macOS 10.10+

``` source
static var slideForward: NSViewController.TransitionOptions { get }
```

## Discussion

- For left-to-right user interface layout direction, the slideLeft animation option.

- For right-to-left user interface layout direction, the slideRight animation option.

## See Also

### Constants

static var crossfade: NSViewController.TransitionOptions

A transition animation that fades the new view in and simultaneously fades the old view out. You can combine this animation option with any of the “slide” options in this enumeration.

static var slideUp: NSViewController.TransitionOptions

A transition animation that slides the old view up while the new view comes into view from the bottom. In other words, both views slide up.

static var slideDown: NSViewController.TransitionOptions

A transition animation that slides the old view down while the new view slides into view from the top. In other words, both views slide down.

static var slideLeft: NSViewController.TransitionOptions

A transition animation that slides the old view to the left while the new view slides into view from the right. In other words, both views slide to the left.

static var slideRight: NSViewController.TransitionOptions

A transition animation that slides the old view to the right while the new view slides into view from the left. In other words, both views slide to the right.

static var slideBackward: NSViewController.TransitionOptions

A transition animation that reflects the user interface layout direction (userInterfaceLayoutDirection) in a “backward” manner, as follows

static var allowUserInteraction: NSViewController.TransitionOptions

A transition animation that allows user interaction during the transition.

