

- Create ML
- MLDataValue
-  MLDataValue.MultiArrayType 

Structure

# MLDataValue.MultiArrayType

A multidimensional array of data values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MultiArrayType
```

## Topics

### Creating an array type

init(MLMultiArray)

init(shape: [Int])

### Getting the array

var mlMultiArray: MLMultiArray

### Getting an element

subscript(Int) -> Double

subscript([Int]) -> Double

### Default Implementations

CustomDebugStringConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

MLDataValueConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- MLDataValueConvertible

## See Also

### Accessing array values

var sequenceValue: MLDataValue.SequenceType?

The underlying sequence.

struct SequenceType

A sequence of data values.

var multiArrayValue: MLDataValue.MultiArrayType?

The underlying multidimensional array.

