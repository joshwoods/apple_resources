

- Core ML
- MLShapedArraySlice
-  init(data:shape:) 

Initializer

# init(data:shape:)

Creates a shaped array with a defined data and shape.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    data: Data,
    shape: [Int]
)
```

Available when `Scalar` conforms to `MLShapedArrayScalar`.

## Parameters 

`data`  

A block of data that initializes the array.

`shape`  

The shape of the array.

## See Also

### Creating a Shaped Array Slice with Data

init(data: Data, shape: [Int], strides: [Int])

Creates a shaped array with defined data, shape, and strides.

