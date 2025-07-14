

- XCUIAutomation
- XCUIElement
-  press(forDuration:thenDragTo:) 

Instance Method

# press(forDuration:thenDragTo:)

Initiates a press-and-hold gesture, then drags to another element.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func press(
    forDuration duration: TimeInterval,
    thenDragTo otherElement: XCUIElement
)
```

## Parameters 

`duration`  

The duration of the initial press-and-hold gesture.

`otherElement`  

The element over which to finish the drag. For example, when reordering table cells, this element is the reorder icon of the destination row.

## Discussion

This interaction is suitable for table-cell reordering and similar operations.

## See Also

### Tapping and pressing

func tap()

Sends a tap event to a hittable point the system computes for the element.

func doubleTap()

Sends a double-tap event to a hittable point the system computes for the element.

func press(forDuration: TimeInterval)

Sends a press-and-hold gesture to a hittable point the system computes for the element, holding for the duration you specify.

func press(forDuration: TimeInterval, thenDragTo: XCUIElement, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Initiates a press-and-hold gesture, drags to another element at a velocity, and holds for a duration, all of which you specify.

