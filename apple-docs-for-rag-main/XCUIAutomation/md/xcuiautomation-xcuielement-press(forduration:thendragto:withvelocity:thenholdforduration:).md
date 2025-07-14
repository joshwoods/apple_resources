

- XCUIAutomation
- XCUIElement
-  press(forDuration:thenDragTo:withVelocity:thenHoldForDuration:) 

Instance Method

# press(forDuration:thenDragTo:withVelocity:thenHoldForDuration:)

Initiates a press-and-hold gesture, drags to another element at a velocity, and holds for a duration, all of which you specify.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(
    forDuration duration: TimeInterval,
    thenDragTo otherElement: XCUIElement,
    withVelocity velocity: XCUIGestureVelocity,
    thenHoldForDuration holdDuration: TimeInterval
)
```

## Parameters 

`duration`  

The duration of the initial press-and-hold gesture.

`otherElement`  

The element over which to finish the drag gesture.

`velocity`  

The speed at which to move from the initial press position to the other element, expressed in pixels per second.

`holdDuration`  

The duration for which to hold the dragged element over the other element.

## See Also

### Tapping and pressing

func tap()

Sends a tap event to a hittable point the system computes for the element.

func doubleTap()

Sends a double-tap event to a hittable point the system computes for the element.

func press(forDuration: TimeInterval)

Sends a press-and-hold gesture to a hittable point the system computes for the element, holding for the duration you specify.

func press(forDuration: TimeInterval, thenDragTo: XCUIElement)

Initiates a press-and-hold gesture, then drags to another element.

