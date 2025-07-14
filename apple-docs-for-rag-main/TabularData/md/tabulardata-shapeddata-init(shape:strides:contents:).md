

- TabularData
- ShapedData
-  init(shape:strides:contents:) 

Initializer

# init(shape:strides:contents:)

Creates a multidimensional shaped array from a one-dimensional array.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    shape: [Int],
    strides: [Int],
    contents: [Element]
)
```

## Parameters 

`shape`  

An integer array that stores the size of each dimension in the corresponding element.

`strides`  

An integer array that stores the number of memory locations that span the length of each dimension in the corresponding element.

`contents`  

A linear array that stores the elements of the multidimensional array.

