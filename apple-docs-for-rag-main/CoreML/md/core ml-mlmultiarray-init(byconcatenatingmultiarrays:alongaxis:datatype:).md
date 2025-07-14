

- Core ML
- MLMultiArray
-  init(byConcatenatingMultiArrays:alongAxis:dataType:) 

Initializer

# init(byConcatenatingMultiArrays:alongAxis:dataType:)

Merges an array of multiarrays into one multiarray along an axis.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init(
    byConcatenatingMultiArrays multiArrays: [MLMultiArray],
    alongAxis axis: Int,
    dataType: MLMultiArrayDataType
)
```

``` source
convenience init(
    concatenating multiArrays: [MLMultiArray],
    axis: Int,
    dataType: MLMultiArrayDataType
)
```

## Parameters 

`multiArrays`  

An MLMultiArray array.

`axis`  

A zero-based axis number the instances in `multiArray` merge along.

`dataType`  

An MLMultiArrayDataType instance that represents the underlying type of all the instances in `multiArrays`.

## Discussion

All multiarray instances in `multiArrays` must have:

- The same data type

- The same number of dimensions

- The same size for each corresponding dimension, except for the concatenation axis

For example, this code concatenates two multiarrays along their first dimension:

```
let multiarray1 = try MLMultiArray(shape: [1, 5, 7], dataType: .int32)
let multiarray2 = try MLMultiArray(shape: [2, 5, 7], dataType: .int32)

// Merge the two multiarrays along the first dimension.
let multiArray3 = MLMultiArray(concatenating: [multiarray1, multiarray2],
                               axis: 0,
                               dataType: .int32)

assert(multiArray3.shape == [3, 5, 7])
```

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

init(pixelBuffer: CVPixelBuffer, shape: [NSNumber])

Creates a multiarray sharing the surface of a pixel buffer.

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

