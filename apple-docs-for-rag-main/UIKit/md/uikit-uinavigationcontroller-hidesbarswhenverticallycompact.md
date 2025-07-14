

- UIKit
- UINavigationController
-  hidesBarsWhenVerticallyCompact 

Instance Property

# hidesBarsWhenVerticallyCompact

A Boolean value indicating whether the navigation controller hides its bars in a vertically compact environment.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var hidesBarsWhenVerticallyCompact: Bool { get set }
```

## Discussion

When the value of this property is true, the navigation controller hides its navigation bar and toolbar when it transitions to a vertically compact environment. Upon returning to a vertically regular environment, the navigation controller automatically shows both bars again. In addition, unhandled taps in the content area cause the navigation controller to show both bars again. The default value of this property is false.

## See Also

### Hiding the navigation bar

var hidesBarsOnTap: Bool

A Boolean value indicating whether the navigation controller allows hiding of its bars using a tap gesture.

var hidesBarsOnSwipe: Bool

A Boolean value indicating whether the navigation bar hides its bars in response to a swipe gesture.

var hidesBarsWhenKeyboardAppears: Bool

A Boolean value indicating whether the navigation controller hides its bars when the keyboard appears.

var isNavigationBarHidden: Bool

A Boolean value that indicates whether the navigation bar is hidden.

var barHideOnTapGestureRecognizer: UITapGestureRecognizer

The gesture recognizer used to hide and show the navigation and toolbar.

var barHideOnSwipeGestureRecognizer: UIPanGestureRecognizer

The gesture recognizer used to hide the navigation bar and toolbar.

