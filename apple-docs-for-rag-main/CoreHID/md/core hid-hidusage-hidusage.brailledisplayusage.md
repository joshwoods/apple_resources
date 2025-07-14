

- Core HID
- HIDUsage
-  HIDUsage.BrailleDisplayUsage 

Enumeration

# HIDUsage.BrailleDisplayUsage

macOS 15.0+

``` source
enum BrailleDisplayUsage
```

## Topics

### Enumeration Cases

case brailleButtons

case brailleDPadCenter

case brailleDPadDown

case brailleDPadLeft

case brailleDPadRight

case brailleDPadUp

case brailleDisplay

case brailleFaceControls

case brailleJoystickCenter

case brailleJoystickDown

case brailleJoystickLeft

case brailleJoystickRight

case brailleJoystickUp

case brailleKeyboardDot1

case brailleKeyboardDot2

case brailleKeyboardDot3

case brailleKeyboardDot4

case brailleKeyboardDot5

case brailleKeyboardDot6

case brailleKeyboardDot7

case brailleKeyboardDot8

case brailleKeyboardLeftSpace

case brailleKeyboardRightSpace

case brailleKeyboardSpace

case brailleLeftControls

case braillePanLeft

case braillePanRight

case brailleRightControls

case brailleRockerDown

case brailleRockerPress

case brailleRockerUp

case brailleRow

case brailleTopControls

case eightDotBrailleCell

case numberOfBrailleCells

case routerKey

case routerSet1

case routerSet2

case routerSet3

case rowRouterKey

case screenReaderControl

case screenReaderIdentifier

case sixDotBrailleCell

### Initializers

init?(rawValue: UInt16)

Creates a new instance with the specified raw value.

### Instance Properties

var rawValue: UInt16

The corresponding value of the raw type.

### Type Aliases

typealias RawValue

The raw type that can be used to represent all values of the conforming type.

### Type Properties

static let page: UInt16

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

