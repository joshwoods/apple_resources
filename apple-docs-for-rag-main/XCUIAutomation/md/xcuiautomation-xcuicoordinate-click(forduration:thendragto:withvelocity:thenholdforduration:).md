

- XCUIAutomation
- XCUICoordinate
-  click(forDuration:thenDragTo:withVelocity:thenHoldForDuration:) 

Instance Method

# click(forDuration:thenDragTo:withVelocity:thenHoldForDuration:)

Clicks and holds for a duration, drags at a velocity, and holds over the other coordinate for a duration, all of which you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func click(
    forDuration duration: TimeInterval,
    thenDragTo otherCoordinate: XCUICoordinate,
    withVelocity velocity: XCUIGestureVelocity,
    thenHoldForDuration holdDuration: TimeInterval
)
```

## Parameters 

`duration`  

The duration of the initial click and hold.

`otherCoordinate`  

The coordinate over which to finish the drag gesture.

`velocity`  

The speed at which to move from the initial click position to the other coordinate, expressed in pixels per second.

`holdDuration`  

The duration for which to hold over the other coordinate after dragging.

## See Also

### Clicking

func click()

Sends a click event at the coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Clicks and holds for a duration you specify, then drags to the other coordinate.

func doubleClick()

Sends a double-click event at the coordinate.

func rightClick()

Sends a Control-click event at the coordinate.

