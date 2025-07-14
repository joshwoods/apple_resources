

- XCUIAutomation
- XCUIElement
-  click() 

Instance Method

# click()

Sends a click event to a hittable point computed for the element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func click()
```

## Discussion

If the element exists within a scrollable view but is offscreen, the framework attempts to scroll the element onscreen before performing the click.

## See Also

### Clicking

func click(forDuration: TimeInterval, thenDragTo: XCUIElement)

Clicks and holds an element for a duration you specify, and then drags it to another element.

func click(forDuration: TimeInterval, thenDragTo: XCUIElement, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Clicks and holds an element for a duration, drags it at a velocity, and holds it over another element for a duration, all of which you specify.

func doubleClick()

Sends a double-click event to a hittable point the system computes for the element.

func rightClick()

Sends a Control-click event to a hittable point the system computes for the element.

