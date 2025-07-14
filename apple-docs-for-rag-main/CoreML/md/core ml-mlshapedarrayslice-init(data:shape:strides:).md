

- Core ML
- MLShapedArraySlice
-  init(data:shape:strides:) 

Initializer

# init(data:shape:strides:)

Creates a shaped array with defined data, shape, and strides.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    data: Data,
    shape: [Int],
    strides: [Int]
)
```

## Parameters 

`data`  

A block of data that initializes the array.

`shape`  

The shape of the array.

`strides`  

The strides of the array.

## See Also

### Creating a Shaped Array Slice with Data

init(data: Data, shape: [Int])

Creates a shaped array with a defined data and shape.

