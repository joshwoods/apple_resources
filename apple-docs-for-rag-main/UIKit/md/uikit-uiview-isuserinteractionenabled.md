

- UIKit
- UIView
-  isUserInteractionEnabled 

Instance Property

# isUserInteractionEnabled

A Boolean value that determines whether user events are ignored and removed from the event queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isUserInteractionEnabled: Bool { get set }
```

## Mentioned in 

Handling rotation gestures

Handling pan gestures

Handling pinch gestures

Handling swipe gestures

Handling long-press gestures

## Discussion

When set to false, touch, press, keyboard, and focus events intended for the view are ignored and removed from the event queue. When set to true, events are delivered to the view normally. The default value of this property is true.

During an animation, user interactions are temporarily disabled for all views involved in the animation, regardless of the value in this property. You can disable this behavior by specifying the allowUserInteraction option when configuring the animation.

Note

Some UIKit subclasses override this property and return a different default value. See the documentation for that class to determine if it returns a different value.

## See Also

### Configuring the event-related behavior

var isMultipleTouchEnabled: Bool

A Boolean value that indicates whether the view receives more than one touch at a time.

var isExclusiveTouch: Bool

A Boolean value that indicates whether the receiver handles touch events exclusively.

