

- Core ML
- MLMultiArray
-  init(pixelBuffer:shape:) 

Initializer

# init(pixelBuffer:shape:)

Creates a multiarray sharing the surface of a pixel buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    pixelBuffer: CVPixelBuffer,
    shape: [NSNumber]
)
```

## Parameters 

`pixelBuffer`  

The pixel buffer owned by the instance.

`shape`  

The shape of the `MLMultiArray`. The last dimension of `shape` must match the pixel buffer’s width. The product of the rest of the dimensions must match the height.

## Discussion

Use this initializer to create an IOSurface-backed `MLMultiArray` that reduces the inference latency by avoiding the buffer copy to and from some compute units.

The instance will own the pixel buffer and release it on the deallocation.

The pixel buffer’s pixel format type must be kCVPixelFormatType_OneComponent16Half. The `MLMultiArray` data type is MLMultiArrayDataType.float16.

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

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

