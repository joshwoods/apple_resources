

- MediaExtension
- MERAWProcessingParameter
-  MERAWProcessingParameter.SubGroup 

Class

# MERAWProcessingParameter.SubGroup

An object that describes a sub group parameter of a RAW processor.

macOS 15.0+

``` source
class SubGroup
```

## Overview

Sub groups are logical groupings of MERAWProcessingParameter objects that should be displayed together in an application user interface.

## Topics

### Creating a sub group parameter object

init(name: String, description: String, parameters: [MERAWProcessingParameter])

Creates a sub group parameter object with the parameters value.

### Properties

var subGroupParameters: [MERAWProcessingParameter]

The array of MERAWProcessingParameter objects in the sub group.

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

class Integer

An object that describes an integer parameter of a RAW processor.

class List

An object that describes a list parameter of a RAW processor.

class ListElement

An object that describes a list element parameter of a RAW processor.

