

- XCUIAutomation
- XCUICoordinate
-  click(forDuration:thenDragTo:) 

Instance Method

# click(forDuration:thenDragTo:)

Clicks and holds for a duration you specify, then drags to the other coordinate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func click(
    forDuration duration: TimeInterval,
    thenDragTo otherCoordinate: XCUICoordinate
)
```

## Parameters 

`duration`  

The duration of the initial click and hold.

`otherCoordinate`  

The coordinate over which to finish the drag gesture.

## See Also

### Clicking

func click()

Sends a click event at the coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Clicks and holds for a duration, drags at a velocity, and holds over the other coordinate for a duration, all of which you specify.

func doubleClick()

Sends a double-click event at the coordinate.

func rightClick()

Sends a Control-click event at the coordinate.

