

- UIKit
- UIFocusUpdateContext
-  previouslyFocusedView 

Instance Property

# previouslyFocusedView

The view that was focused before the focus update.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
weak var previouslyFocusedView: UIView? { get }
```

## Discussion

If your app targets tvOS 10 and later, use previouslyFocusedItem instead.

This property returns `nil` when no view was previously focused, such as when setting the initial focus.

## See Also

### Locating focus direction

var nextFocusedView: UIView?

The view that takes the focus after the focus update.

var focusHeading: UIFocusHeading

The heading in which the focus update is occurring.

struct UIFocusHeading

The general type of an event.

