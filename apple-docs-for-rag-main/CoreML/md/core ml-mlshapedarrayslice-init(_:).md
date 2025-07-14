

- Core ML
- MLShapedArraySlice
-  init(\_:) 

Initializer

# init(\_:)

Creates a new MLShapedArraySlice using a `MLMultiArray` as a backing storage.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 1.0+watchOS 11.0+

``` source
init(_ multiArray: MLMultiArray)
```

## Parameters 

`multiArray`  

The `MLMultiArray` object.

## Discussion

Use this initializer to access `MLMultiArray` through `MLShapedArray` interface.

Mutating operations trigger copy-on-write. Non-mutating operations access the `MLMultiArray`’s backing storage including the pixel buffer.

## See Also

### Creating a Shaped Array Slice from Another Type

init&lt;S>(concatenating: S, alongAxis: Int)

Merges a sequence of shaped arrays into one shaped array along an axis.

