

- Core ML
- MLMultiArray
-  init(dataPointer:shape:dataType:strides:deallocator:) 

Initializer

# init(dataPointer:shape:dataType:strides:deallocator:)

Creates a multiarray from a data pointer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
init(
    dataPointer: UnsafeMutableRawPointer,
    shape: [NSNumber],
    dataType: MLMultiArrayDataType,
    strides: [NSNumber],
    deallocator: ((UnsafeMutableRawPointer) -> Void)? = nil
) throws
```

## Parameters 

`dataPointer`  

A pointer to data in memory.

`shape`  

An integer array with an element for each dimension. An element represents the size of the corresponding dimension.

`dataType`  

An MLMultiArrayDataType instance that represents the pointer’s data type.

`strides`  

An integer array with an element for each dimension. An element represents the number of memory locations that span the length of the corresponding dimension.

`deallocator`  

In Swift, a closure the multiarray calls in its deinitializer. In Objective-C, a block the multiarray calls in its dealloc method.

## Discussion

The caller is responsible for freeing the memory the `dataPointer` points to, by providing a `deallocator` closure.

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

convenience init(byConcatenatingMultiArrays: [MLMultiArray], alongAxis: Int, dataType: MLMultiArrayDataType)

Merges an array of multiarrays into one multiarray along an axis.

init(pixelBuffer: CVPixelBuffer, shape: [NSNumber])

Creates a multiarray sharing the surface of a pixel buffer.

enum MLMultiArrayDataType

Constants that define the underlying element types a multiarray can store.

