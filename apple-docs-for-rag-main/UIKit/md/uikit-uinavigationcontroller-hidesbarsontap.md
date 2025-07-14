

- UIKit
- UINavigationController
-  hidesBarsOnTap 

Instance Property

# hidesBarsOnTap

A Boolean value indicating whether the navigation controller allows hiding of its bars using a tap gesture.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hidesBarsOnTap: Bool { get set }
```

## Discussion

When the value of this property is true, the navigation controller toggles the hiding and showing of its navigation bar and toolbar in response to an otherwise unhandled tap in the content area. The default value of this property is false.

## See Also

### Hiding the navigation bar

var hidesBarsOnSwipe: Bool

A Boolean value indicating whether the navigation bar hides its bars in response to a swipe gesture.

var hidesBarsWhenVerticallyCompact: Bool

A Boolean value indicating whether the navigation controller hides its bars in a vertically compact environment.

var hidesBarsWhenKeyboardAppears: Bool

A Boolean value indicating whether the navigation controller hides its bars when the keyboard appears.

var isNavigationBarHidden: Bool

A Boolean value that indicates whether the navigation bar is hidden.

var barHideOnTapGestureRecognizer: UITapGestureRecognizer

The gesture recognizer used to hide and show the navigation and toolbar.

var barHideOnSwipeGestureRecognizer: UIPanGestureRecognizer

The gesture recognizer used to hide the navigation bar and toolbar.

