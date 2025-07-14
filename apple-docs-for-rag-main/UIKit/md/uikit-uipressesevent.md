

- UIKit
-  UIPressesEvent 

Class

# UIPressesEvent

An event that describes the state of a set of physical buttons that are available to the device, such as those on an associated remote or game controller.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
class UIPressesEvent
```

## Topics

### Reading the event button presses

var allPresses: Set&lt;UIPress>

The state of all physical buttons in the event.

func presses(for: UIGestureRecognizer) -> Set&lt;UIPress>

Returns the state of all physical buttons in the event that are associated with a particular gesture recognizer.

## Relationships

### Inherits From

- UIEvent

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Button presses

class UIPress

An object that represents the presence or movement of a button press on the screen for a particular event.

