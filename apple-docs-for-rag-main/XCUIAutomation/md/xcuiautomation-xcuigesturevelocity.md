

- XCUIAutomation
-  XCUIGestureVelocity 

Structure

# XCUIGestureVelocity

A value that describes how fast a gesture moves across the screen, in pixels per second.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOSXcode 16.3+

``` source
struct XCUIGestureVelocity
```

## Topics

### Creating a gesture velocity

init(CGFloat)

Creates a gesture velocity, expressed as a float.

init(integerLiteral: Int)

Creates a gesture velocity with an integer value.

init(floatLiteral: XCUIGestureVelocity.FloatLiteralType)

Creates a gesture velocity with a float value.

init(rawValue: CGFloat)

Creates a gesture velocity with a raw value, expressed as a float.

typealias IntegerLiteralType

A type that specifies a gesture velocity with an integer literal.

typealias FloatLiteralType

The native type that specifies the gesture velocity value.

### Using typical gesture velocities

static let `default`: XCUIGestureVelocity

A value representing a default gesture velocity.

static let fast: XCUIGestureVelocity

A value representing a fast gesture velocity.

static let slow: XCUIGestureVelocity

A value representing a slow gesture velocity.

### Default Implementations

Equatable Implementations

ExpressibleByFloatLiteral Implementations

ExpressibleByIntegerLiteral Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- ExpressibleByFloatLiteral
- ExpressibleByIntegerLiteral
- Hashable
- RawRepresentable
- Sendable

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

func rotate(CGFloat, withVelocity: CGFloat)

Sends a rotation gesture with two touches.

