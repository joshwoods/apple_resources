

- XCUIAutomation
- XCUICoordinate
-  doubleTap() 

Instance Method

# doubleTap()

Sends a double-tap event at the coordinate.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func doubleTap()
```

## Discussion

This method is available in iOS and for Touch Bar interactions in macOS.

## See Also

### Tapping and pressing

func tap()

Sends a tap event at the coordinate.

func press(forDuration: TimeInterval)

Initiates a press-and-hold gesture at the coordinate, holding for the duration you specify.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Initiates a press-and-hold gesture at the coordinate, then drags to another coordinate.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Initiates a press-and-hold gesture, drags to another coordinate with a velocity you specify, and holds for a duration you specify.

