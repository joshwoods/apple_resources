

- XCUIAutomation
- XCUICoordinate
-  rightClick() 

Instance Method

# rightClick()

Sends a Control-click event at the coordinate.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func rightClick()
```

## See Also

### Clicking

func click()

Sends a click event at the coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Clicks and holds for a duration you specify, then drags to the other coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Clicks and holds for a duration, drags at a velocity, and holds over the other coordinate for a duration, all of which you specify.

func doubleClick()

Sends a double-click event at the coordinate.

