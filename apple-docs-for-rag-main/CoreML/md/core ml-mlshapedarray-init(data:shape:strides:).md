

- Core ML
- MLShapedArray
-  init(data:shape:strides:) 

Initializer

# init(data:shape:strides:)

Creates a shaped array from a block of data, a shape, and strides.

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

The block of data that holds the contents of the shaped array.

`shape`  

The shape of the array.

`strides`  

The strides of the array.

## See Also

### Creating a shaped array from data

init(data: Data, shape: [Int])

Creates a shaped array from a block of data and a shape.

