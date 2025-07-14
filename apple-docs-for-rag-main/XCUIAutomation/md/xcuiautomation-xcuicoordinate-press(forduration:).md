

- XCUIAutomation
- XCUICoordinate
-  press(forDuration:) 

Instance Method

# press(forDuration:)

Initiates a press-and-hold gesture at the coordinate, holding for the duration you specify.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(forDuration duration: TimeInterval)
```

## Parameters 

`duration`  

The duration of the press, in seconds.

## See Also

### Tapping and pressing

func tap()

Sends a tap event at the coordinate.

func doubleTap()

Sends a double-tap event at the coordinate.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Initiates a press-and-hold gesture at the coordinate, then drags to another coordinate.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Initiates a press-and-hold gesture, drags to another coordinate with a velocity you specify, and holds for a duration you specify.

