

- MediaExtension
- MERAWProcessingParameter
-  MERAWProcessingParameter.Boolean 

Class

# MERAWProcessingParameter.Boolean

An object that describes a Boolean parameter of a RAW processor.

macOS 15.0+

``` source
class Boolean
```

## Topics

### Creating a boolean parameter object

convenience init(name: String, key: String, description: String, initialValue: Bool, neutralValue: Bool?, cameraValue: Bool?)

Creates a Boolean parameter object.

### Properties

var currentValue: Bool

Get or set the current value for this parameter.

var initialValue: Bool

The initial value for this parameter as defined in the sequence metadata.

### Instance Properties

var cameraValue: Bool?

var neutralValue: Bool?

## Relationships

### Inherits From

- MERAWProcessingParameter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Processing parameters

class FloatingPoint

An object that describes a floating-point parameter of a RAW processor.

class Integer

An object that describes an integer parameter of a RAW processor.

class List

An object that describes a list parameter of a RAW processor.

class ListElement

An object that describes a list element parameter of a RAW processor.

class SubGroup

An object that describes a sub group parameter of a RAW processor.

