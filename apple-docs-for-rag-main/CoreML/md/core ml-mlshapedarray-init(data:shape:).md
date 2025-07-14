

- Core ML
- MLShapedArray
-  init(data:shape:) 

Initializer

# init(data:shape:)

Creates a shaped array from a block of data and a shape.

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

The block of data that holds the contents of the shaped array.

`shape`  

The shape of the array.

## See Also

### Creating a shaped array from data

init(data: Data, shape: [Int], strides: [Int])

Creates a shaped array from a block of data, a shape, and strides.

