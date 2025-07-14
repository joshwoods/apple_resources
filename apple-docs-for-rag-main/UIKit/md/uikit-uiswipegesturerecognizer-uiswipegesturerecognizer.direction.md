

- UIKit
- UISwipeGestureRecognizer
-  UISwipeGestureRecognizer.Direction 

Structure

# UISwipeGestureRecognizer.Direction

The direction of the swipe.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct Direction
```

## Topics

### Constants

static var right: UISwipeGestureRecognizer.Direction

The touch or touches swipe to the right.

static var left: UISwipeGestureRecognizer.Direction

The touch or touches swipe to the left.

static var up: UISwipeGestureRecognizer.Direction

The touch or touches swipe upward.

static var down: UISwipeGestureRecognizer.Direction

The touch or touches swipe downward.

### Initializers

init(rawValue: UInt)

Creates a swipe direction structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring the gesture

var direction: UISwipeGestureRecognizer.Direction

The permitted direction of the swipe for this gesture recognizer.

var numberOfTouchesRequired: Int

The number of touches necessary for swipe recognition.

