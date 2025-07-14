

- UIKit
- UINavigationController
-  isNavigationBarHidden 

Instance Property

# isNavigationBarHidden

A Boolean value that indicates whether the navigation bar is hidden.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isNavigationBarHidden: Bool { get set }
```

## Discussion

If true, the navigation bar is hidden. The default value is false. Setting this property changes the visibility of the navigation bar without animating the changes. If you want to animate the change, use the setNavigationBarHidden(_:animated:)method instead.

## See Also

### Hiding the navigation bar

var hidesBarsOnTap: Bool

A Boolean value indicating whether the navigation controller allows hiding of its bars using a tap gesture.

var hidesBarsOnSwipe: Bool

A Boolean value indicating whether the navigation bar hides its bars in response to a swipe gesture.

var hidesBarsWhenVerticallyCompact: Bool

A Boolean value indicating whether the navigation controller hides its bars in a vertically compact environment.

var hidesBarsWhenKeyboardAppears: Bool

A Boolean value indicating whether the navigation controller hides its bars when the keyboard appears.

var barHideOnTapGestureRecognizer: UITapGestureRecognizer

The gesture recognizer used to hide and show the navigation and toolbar.

var barHideOnSwipeGestureRecognizer: UIPanGestureRecognizer

The gesture recognizer used to hide the navigation bar and toolbar.

