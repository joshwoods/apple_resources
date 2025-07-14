

- Core ML
-  MLMultiArrayDataType 

Enumeration

# MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum MLMultiArrayDataType
```

## Overview

All elements of an MLMultiArray instance must be of the same type and must be defined in MLMultiArrayDataType.

## Topics

### Multiarray Data Types

case int32

Designates the multiarray’s elements as 32-bit integers.

case float16

Designates the multiarray’s elements as 16-bit floats.

case float32

Designates the multiarray’s elements as 32-bit floats.

case double

Designates the multiarray’s elements as doubles.

static var float: MLMultiArrayDataType

Designates the multiarray’s elements as floats.

static var float64: MLMultiArrayDataType

Designates the multiarray’s elements as 64-bit floats.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating a Multiarray

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of integers.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of floats.

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of doubles.

init(shape: [NSNumber], dataType: MLMultiArrayDataType) throws

Creates a multidimensional array with a shape and type.

convenience init&lt;ShapedArray>(ShapedArray)

Creates a multiarray from a shaped array.

init(dataPointer: UnsafeMutableRawPointer, shape: [NSNumber], dataType: MLMultiArrayDataType, strides: [NSNumber], deallocator: ((UnsafeMutableRawPointer) -> Void)?) throws

Creates a multiarray from a data pointer.

convenience init(byConcatenatingMultiArrays: [MLMultiArray], alongAxis: Int, dataType: MLMultiArrayDataType)

Merges an array of multiarrays into one multiarray along an axis.

init(pixelBuffer: CVPixelBuffer, shape: [NSNumber])

Creates a multiarray sharing the surface of a pixel buffer.

