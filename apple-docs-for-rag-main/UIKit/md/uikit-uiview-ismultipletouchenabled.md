

- UIKit
- UIView
-  isMultipleTouchEnabled 

Instance Property

# isMultipleTouchEnabled

A Boolean value that indicates whether the view receives more than one touch at a time.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
var isMultipleTouchEnabled: Bool { get set }
```

## Discussion

When set to true, the view receives all touches associated with a multi-touch sequence and starting within the view’s bounds. When set to false, the view receives only the first touch event in a multi-touch sequence that start within the view’s bounds. The default value of this property is false.

Note

This property does not affect the gesture recognizers attached to the view. Gesture recognizers receive all touches that occur in the view.

Other views in the same window can still receive touch events when this property is false. If you want this view to handle multi-touch events exclusively, set the values of both this property and the isExclusiveTouch property to true. This property does not prevent a view from being asked to handle multiple touches. For example, two subviews may both forward their touches to a common parent, such as a window or the root view of a view controller. This property determines how many touches initially targeting the view are delivered to that view.

## See Also

### Configuring the event-related behavior

var isUserInteractionEnabled: Bool

A Boolean value that determines whether user events are ignored and removed from the event queue.

var isExclusiveTouch: Bool

A Boolean value that indicates whether the receiver handles touch events exclusively.

