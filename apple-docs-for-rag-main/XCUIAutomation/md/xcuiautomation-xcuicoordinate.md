

- XCUIAutomation
-  XCUICoordinate 

Class

# XCUICoordinate

A location on screen relative to a UI element.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
class XCUICoordinate
```

## Overview

Coordinates are dynamic, like the elements to which they refer, and may compute different screen locations at different times, or be invalid if the element they reference doesn’t exist.

## Topics

### Getting coordinate properties

var referencedElement: XCUIElement

The element that the coordinate is based on, either directly or through the coordinate from which it was derived.

var screenPoint: CGPoint

The dynamically computed value of the coordinate’s location on screen.

### Moving the pointer

func hover()

Moves the pointer to the coordinate.

### Clicking

func click()

Sends a click event at the coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Clicks and holds for a duration you specify, then drags to the other coordinate.

func click(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Clicks and holds for a duration, drags at a velocity, and holds over the other coordinate for a duration, all of which you specify.

func doubleClick()

Sends a double-click event at the coordinate.

func rightClick()

Sends a Control-click event at the coordinate.

### Scrolling

func scroll(byDeltaX: CGFloat, deltaY: CGFloat)

Scrolls the view by the number of x and y pixels you specify.

### Tapping and pressing

func tap()

Sends a tap event at the coordinate.

func doubleTap()

Sends a double-tap event at the coordinate.

func press(forDuration: TimeInterval)

Initiates a press-and-hold gesture at the coordinate, holding for the duration you specify.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate)

Initiates a press-and-hold gesture at the coordinate, then drags to another coordinate.

func press(forDuration: TimeInterval, thenDragTo: XCUICoordinate, withVelocity: XCUIGestureVelocity, thenHoldForDuration: TimeInterval)

Initiates a press-and-hold gesture, drags to another coordinate with a velocity you specify, and holds for a duration you specify.

### Performing gestures

func swipeLeft()

Sends a swipe-left gesture.

func swipeLeft(velocity: XCUIGestureVelocity)

Sends a swipe-left gesture with a velocity you specify.

func swipeRight()

Sends a swipe-right gesture.

func swipeRight(velocity: XCUIGestureVelocity)

Sends a swipe-right gesture with a velocity you specify.

func swipeUp()

Sends a swipe-up gesture.

func swipeUp(velocity: XCUIGestureVelocity)

Sends a swipe-up gesture with a velocity you specify.

func swipeDown()

Sends a swipe-down gesture.

func swipeDown(velocity: XCUIGestureVelocity)

Sends a swipe-down gesture with a velocity you specify.

### Creating relative coordinates

func withOffset(CGVector) -> XCUICoordinate

Creates a new coordinate with an absolute offset in points from the original coordinate.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### UI elements

class XCUIElement

A UI element in an application.

protocol XCUIElementAttributes

Attributes exposed by UI elements.

protocol XCUIElementSnapshot

A set of attributes to express a snapshot of an element’s attributes and descendant user interface hierarchy.

protocol XCUIElementSnapshotProviding

A method to capture a snapshot of an element’s attributes and descendant user interface hierarchy.

