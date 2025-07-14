

- XCUIAutomation
- XCUIElement
-  press(forDuration:) 

Instance Method

# press(forDuration:)

Sends a press-and-hold gesture to a hittable point the system computes for the element, holding for the duration you specify.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(forDuration duration: TimeInterval)
```

## Parameters 

`duration`  

The duration of the press, in seconds.

## Discussion

If the element exists within a scrollable view but is offscreen, XCTest attempts to scroll the element onscreen before performing the press.

## See Also

### Tapping and pressing

func tap()

Sends a tap event to a hittable point the system computes for the element.

func doubleTap()

Sends a double-tap event to a hittable point the system computes for the element.

func press(forDuration: TimeInterval, thenDragTo: XCUIElement)

Initiates a press-and-hold gesture, then drags to another element.

func press(forDuration: TimeInterval, thenDragTo: XCUIElement, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Initiates a press-and-hold gesture, drags to another element at a velocity, and holds for a duration, all of which you specify.

