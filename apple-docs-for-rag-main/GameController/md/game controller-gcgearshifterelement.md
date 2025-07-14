

- Game Controller
-  GCGearShifterElement 

Class

# GCGearShifterElement

An element that represents either a pattern or a sequential gear shift.

Mac Catalyst 16.0+macOS 13.0+

``` source
class GCGearShifterElement
```

## Topics

### Accessing input values

var patternInput: (any GCSwitchPositionInput)?

The input object for a pattern gear shift.

var sequentialInput: (any GCRelativeInput)?

The input object for a sequential gear shift.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- GCPhysicalInputElement
- Hashable
- NSObjectProtocol

## See Also

### Gear shifter elements

protocol GCAxisInput

The common properties of inputs that provide absolute values along an axis with a fixed origin.

protocol GCRelativeInput

The common properties of inputs that provide positions along an axis that are relative to the previous position.

