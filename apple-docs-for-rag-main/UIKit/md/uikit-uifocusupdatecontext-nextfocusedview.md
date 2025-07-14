

- UIKit
- UIFocusUpdateContext
-  nextFocusedView 

Instance Property

# nextFocusedView

The view that takes the focus after the focus update.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
weak var nextFocusedView: UIView? { get }
```

## Discussion

If your app targets tvOS 10 and later, use nextFocusedItem instead.

This property returns `nil` if no view will be focused after the update.

## See Also

### Locating focus direction

var previouslyFocusedView: UIView?

The view that was focused before the focus update.

var focusHeading: UIFocusHeading

The heading in which the focus update is occurring.

struct UIFocusHeading

The general type of an event.

