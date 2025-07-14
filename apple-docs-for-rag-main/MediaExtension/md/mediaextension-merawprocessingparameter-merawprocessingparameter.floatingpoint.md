

- MediaExtension
- MERAWProcessingParameter
-  MERAWProcessingParameter.FloatingPoint 

Class

# MERAWProcessingParameter.FloatingPoint

An object that describes a floating-point parameter of a RAW processor.

macOS 15.0+

``` source
class FloatingPoint
```

## Topics

### Creating a floating-point parameter object

convenience init(name: String, key: String, description: String, initialValue: Float, maximum: Float, minimum: Float, neutralValue: Float?, cameraValue: Float?)

Creates a floating-point parameter object.

### Properties

var currentValue: Float

Get or set the current value for this parameter.

var initialValue: Float

The initial value for this parameter as defined in the sequence metadata.

var maximumValue: Float

The maximum value for this parameter.

var minimumValue: Float

The minimum value for this parameter.

### Instance Properties

var cameraValue: Float?

var neutralValue: Float?

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

class Integer

An object that describes an integer parameter of a RAW processor.

class List

An object that describes a list parameter of a RAW processor.

class ListElement

An object that describes a list element parameter of a RAW processor.

class SubGroup

An object that describes a sub group parameter of a RAW processor.

