

- UIKit
- UIEvent
-  allTouches 

Instance Property

# allTouches

All touches associated with the event.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allTouches: Set? { get }
```

## Return Value

A set of UITouch objects representing all touches associated with the event.

## Discussion

If the touches of the event originate in different views and windows, the UITouch objects obtained from this method will be associated with different responder objects.

## See Also

### Getting the touches for an event

func touches(for: UIView) -> Set&lt;UITouch>?

Returns the touch objects from the event that belong to the specified given view.

func touches(for: UIWindow) -> Set&lt;UITouch>?

Returns the touch objects from the event that belong to the specified window.

func coalescedTouches(for: UITouch) -> [UITouch]?

Returns all of the touches associated with the specified main touch.

func predictedTouches(for: UITouch) -> [UITouch]?

Returns an array of touches that are predicted to occur for the specified touch.

