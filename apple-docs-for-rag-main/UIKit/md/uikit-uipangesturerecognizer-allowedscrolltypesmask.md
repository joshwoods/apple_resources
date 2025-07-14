

- UIKit
- UIPanGestureRecognizer
-  allowedScrollTypesMask 

Instance Property

# allowedScrollTypesMask

A scroll type mask that enables recognition of scroll events.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
var allowedScrollTypesMask: UIScrollTypeMask { get set }
```

## Discussion

Setting this mask enables the pan gesture to recognize scroll events, like a mouse scroll movement or a two-finger scroll on a track pad. See UIScrollType.

Note

Setting this property doesn’t disable scrolling through touches. To disable touch scrolling, return false from gestureRecognizer(_:shouldReceive:) or set the allowedTouchTypes to an empty array.

## See Also

### Tracking scroll events

struct UIScrollTypeMask

A bit mask identifying the scroll type of a pan gesture.

enum UIScrollType

Constants that define the type of the scroll.

