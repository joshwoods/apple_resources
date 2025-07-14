

- UIKit
- UIEvent
-  UIEvent.ButtonMask 

Structure

# UIEvent.ButtonMask

Constants that indicate which input-device buttons are pressed.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
struct ButtonMask
```

## Topics

### Creating button masks

init(rawValue: Int)

Creates a button mask with the specified raw value.

static func button(Int) -> UIEvent.ButtonMask

Creates a button mask from the specified button index.

### Accessing button masks

static var primary: UIEvent.ButtonMask

A constant that represents the primary button on the input device.

static var secondary: UIEvent.ButtonMask

A constant that represents the secondary button on the input device.

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

### Getting the button mask

var buttonMask: UIEvent.ButtonMask

A bit mask that represents which input-device buttons are pressed for the current event.

