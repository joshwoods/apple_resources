

- XCUIAutomation
- XCUIElement
-  rotate(\_:withVelocity:) 

Instance Method

# rotate(\_:withVelocity:)

Sends a rotation gesture with two touches.

iOSiPadOSMac CatalystwatchOSXcode 16.3+

``` source
@MainActor
func rotate(
    _ rotation: CGFloat,
    withVelocity velocity: CGFloat
)
```

## Parameters 

`rotation`  

The rotation of the gesture in radians.

`velocity`  

The velocity of the rotation gesture in radians per second.

## Discussion

The system makes a best effort to synthesize the requested rotation and velocity, but absolute accuracy isn’t guaranteed. Some values may not be possible based on the size of the element’s frame, and they result in test failures.

## See Also

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

func pinch(withScale: CGFloat, velocity: CGFloat)

Sends a pinching gesture with two touches.

struct XCUIGestureVelocity

A value that describes how fast a gesture moves across the screen, in pixels per second.

