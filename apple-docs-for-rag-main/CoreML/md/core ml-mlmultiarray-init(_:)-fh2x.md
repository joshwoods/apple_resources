

- Core ML
- MLMultiArray
-  init(\_:) 

Initializer

# init(\_:)

Creates a multiarray from a collection of floats.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
convenience init(_ data: C) throws where C : Collection, C.Element == Float
```

## Parameters 

`data`  

A Collection of Float values.

## Discussion

Use this initializer to create a multiarray from a collection of Float values, such as an array.

```
let floats: [Float] = [1.41, 1.73, 2.72, 3.14]
let floatMultiarray = try MLMultiArray(floats)
```

## See Also

### Creating a Multiarray

convenience init&lt;C>(C) throws

Creates a multiarray from a collection of integers.

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

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

