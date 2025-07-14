

- XCUIAutomation
- XCUIElement
-  swipeLeft(velocity:) 

Instance Method

# swipeLeft(velocity:)

Sends a swipe-left gesture with a velocity you specify.

iOSiPadOSMac CatalystmacOSvisionOSwatchOSXcode 16.3+

``` source
@MainActor
func swipeLeft(velocity: XCUIGestureVelocity)
```

## Parameters 

`velocity`  

The speed at which to perform the swipe-left gesture, expressed in pixels per second.

## See Also

### Performing gestures

func swipeLeft()

Sends a swipe-left gesture.

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

func rotate(CGFloat, withVelocity: CGFloat)

Sends a rotation gesture with two touches.

struct XCUIGestureVelocity

A value that describes how fast a gesture moves across the screen, in pixels per second.

