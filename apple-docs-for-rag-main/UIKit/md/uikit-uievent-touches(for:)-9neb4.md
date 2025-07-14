

- UIKit
- UIEvent
-  touches(for:) 

Instance Method

# touches(for:)

Returns the touch objects from the event that belong to the specified given view.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func touches(for view: UIView) -> Set?
```

## Parameters 

`view`  

The UIView object in which the touches originally occurred.

## Return Value

A set of UITouch objects representing the touches that belong to the specified view.

## See Also

### Getting the touches for an event

var allTouches: Set&lt;UITouch>?

All touches associated with the event.

func touches(for: UIWindow) -> Set&lt;UITouch>?

Returns the touch objects from the event that belong to the specified window.

func coalescedTouches(for: UITouch) -> [UITouch]?

Returns all of the touches associated with the specified main touch.

func predictedTouches(for: UITouch) -> [UITouch]?

Returns an array of touches that are predicted to occur for the specified touch.

