

- MediaExtension
- MERAWProcessingParameter
-  MERAWProcessingParameter.ListElement 

Class

# MERAWProcessingParameter.ListElement

An object that describes a list element parameter of a RAW processor.

macOS 15.0+

``` source
class ListElement
```

## Overview

The `MERAWProcessingParameterListElement` protocol provides an interface for `VideoToolbox` to query descriptions of the different elements in a parameter list for a list element in a `MERAWProcessingParameter`. A distinct `MERAWProcessingParameterListElement` is created for each list element.

## Topics

### Creating a list element parameter object

init(name: String, description: String, elementID: Int)

Creates a list element parameter object with the element id value.

### Properties

var listElementID: Int

A unique number in the list which represents this list option.

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

class SubGroup

An object that describes a sub group parameter of a RAW processor.

