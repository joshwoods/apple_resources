

- XCUIAutomation
- XCUICoordinate
-  press(forDuration:thenDragTo:withVelocity:thenHoldForDuration:) 

Instance Method

# press(forDuration:thenDragTo:withVelocity:thenHoldForDuration:)

Initiates a press-and-hold gesture, drags to another coordinate with a velocity you specify, and holds for a duration you specify.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(
    forDuration duration: TimeInterval,
    thenDragTo otherCoordinate: XCUICoordinate,
    withVelocity velocity: XCUIGestureVelocity,
    thenHoldForDuration holdDuration: TimeInterval
)
```

## Parameters 

`duration`  

The duration of the initial press-and-hold gesture.

`otherCoordinate`  

The coordinate over which to finish the drag.

`velocity`  

The speed at which to move from the initial press position to the other element, expressed in pixels per second.

`holdDuration`  

The duration for which to hold over the other coordinate after dragging.

## Discussion

This method is available in iOS and for Touch Bar interactions in macOS.

## See Also

### Tapping and pressing

func tap()

Sends a tap event at the coordinate.

func doubleTap()

Sends a double-tap event at the coordinate.

func press(forDuration: TimeInterval)

Initiates a press-and-hold gesture at the coordinate, holding for the duration you specify.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Initiates a press-and-hold gesture at the coordinate, then drags to another coordinate.

