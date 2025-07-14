

- UIKit
- UIFocusUpdateContext
-  focusHeading 

Instance Property

# focusHeading

The heading in which the focus update is occurring.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var focusHeading: UIFocusHeading { get }
```

## Discussion

To view all the possible focus heading directions, see the UIFocusHeading data type.

## See Also

### Locating focus direction

var previouslyFocusedView: UIView?

The view that was focused before the focus update.

var nextFocusedView: UIView?

The view that takes the focus after the focus update.

struct UIFocusHeading

The general type of an event.

