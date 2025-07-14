

- UIKit
- UIView
-  isExclusiveTouch 

Instance Property

# isExclusiveTouch

A Boolean value that indicates whether the receiver handles touch events exclusively.

iOSiPadOSMac CatalystvisionOS

``` source
@MainActor
var isExclusiveTouch: Bool { get set }
```

## Discussion

Setting this property to true causes the receiver to block the delivery of touch events to other views in the same window. The default value of this property is false.

## See Also

### Configuring the event-related behavior

var isUserInteractionEnabled: Bool

A Boolean value that determines whether user events are ignored and removed from the event queue.

var isMultipleTouchEnabled: Bool

A Boolean value that indicates whether the view receives more than one touch at a time.

