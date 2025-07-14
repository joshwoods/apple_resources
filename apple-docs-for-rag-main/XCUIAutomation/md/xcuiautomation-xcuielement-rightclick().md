

- XCUIAutomation
- XCUIElement
-  rightClick() 

Instance Method

# rightClick()

Sends a Control-click event to a hittable point the system computes for the element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func rightClick()
```

## Discussion

If the element exists within a scrollable view but is offscreen, XCTest attempts to scroll the element onscreen before performing the Control-click.

## See Also

### Clicking

func click()

Sends a click event to a hittable point computed for the element.

func click(forDuration: TimeInterval, thenDragTo: XCUIElement)

Clicks and holds an element for a duration you specify, and then drags it to another element.

func click(forDuration: TimeInterval, thenDragTo: XCUIElement, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Clicks and holds an element for a duration, drags it at a velocity, and holds it over another element for a duration, all of which you specify.

func doubleClick()

Sends a double-click event to a hittable point the system computes for the element.

