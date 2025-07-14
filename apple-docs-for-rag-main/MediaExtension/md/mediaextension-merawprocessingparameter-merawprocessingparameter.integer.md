

- MediaExtension
- MERAWProcessingParameter
-  MERAWProcessingParameter.Integer 

Class

# MERAWProcessingParameter.Integer

An object that describes an integer parameter of a RAW processor.

macOS 15.0+

``` source
class Integer
```

## Topics

### Creating an integer parameter object

convenience init(name: String, key: String, description: String, initialValue: Int, maximum: Int, minimum: Int, neutralValue: Int?, cameraValue: Int?)

Creates an integer parameter object.

### Properties

var currentValue: Int

Get or set the current value for this parameter.

var initialValue: Int

The initial value for this parameter as defined in the sequence metadata.

var maximumValue: Int

The maximum value for this parameter.

var minimumValue: Int

The minimum value for this parameter.

### Instance Properties

var cameraValue: Int?

var neutralValue: Int?

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

class Boolean

An object that describes a Boolean parameter of a RAW processor.

class FloatingPoint

An object that describes a floating-point parameter of a RAW processor.

class List

An object that describes a list parameter of a RAW processor.

class ListElement

An object that describes a list element parameter of a RAW processor.

class SubGroup

An object that describes a sub group parameter of a RAW processor.

