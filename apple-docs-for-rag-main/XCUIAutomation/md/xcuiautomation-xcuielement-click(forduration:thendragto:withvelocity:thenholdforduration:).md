

- XCUIAutomation
- XCUIElement
-  click(forDuration:thenDragTo:withVelocity:thenHoldForDuration:) 

Instance Method

# click(forDuration:thenDragTo:withVelocity:thenHoldForDuration:)

Clicks and holds an element for a duration, drags it at a velocity, and holds it over another element for a duration, all of which you specify.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOSXcode 16.3+

``` source
@MainActor
func click(
    forDuration duration: TimeInterval,
    thenDragTo otherElement: XCUIElement,
    withVelocity velocity: XCUIGestureVelocity,
    thenHoldForDuration holdDuration: TimeInterval
)
```

## Parameters 

`duration`  

The duration of the initial click and hold.

`otherElement`  

The element over which to finish the drag.

`velocity`  

The speed at which to move from the initial click position to the other element, expressed in pixels per second.

`holdDuration`  

The duration for which to hold the dragged element over the other element.

## Discussion

Specify a duration long enough to initiate a drag operation. If the element exists within a scrollable view but is offscreen, the framework attempts to scroll the element onscreen before performing the click.

## See Also

### Clicking

func click()

Sends a click event to a hittable point computed for the element.

func click(forDuration: TimeInterval, thenDragTo: XCUIElement)

Clicks and holds an element for a duration you specify, and then drags it to another element.

func doubleClick()

Sends a double-click event to a hittable point the system computes for the element.

func rightClick()

Sends a Control-click event to a hittable point the system computes for the element.

