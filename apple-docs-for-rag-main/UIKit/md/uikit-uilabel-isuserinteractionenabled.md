

- UIKit
- UILabel
-  isUserInteractionEnabled 

Instance Property

# isUserInteractionEnabled

A Boolean value that determines whether the system ignores and removes user events for this label from the event queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isUserInteractionEnabled: Bool { get set }
```

## Discussion

UILabel inherits this property from the UIView parent class. This class changes the default value of this property to false.

## See Also

### Related Documentation

var isUserInteractionEnabled: Bool

A Boolean value that determines whether user events are ignored and removed from the event queue.

### Accessing additional attributes

clipsToBounds

A Boolean value that determines whether subviews are confined to the bounds of the view.

