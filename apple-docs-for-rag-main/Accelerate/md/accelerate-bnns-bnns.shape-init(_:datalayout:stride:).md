

- Accelerate
- BNNS
- BNNS.Shape
-  init(\_:dataLayout:stride:) 

Initializer

# init(\_:dataLayout:stride:)

Returns a new shape with the specified size, data layout, and stride.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(
    _ size: [Int],
    dataLayout: BNNS.DataLayout? = nil,
    stride: [Int]? = nil
)
```

## Parameters 

`size`  

An array that specifies the number of values in each dimension.

`dataLayout`  

The number of dimensions of the array, and how it stores the data.

`stride`  

An array specifying the increment, in values, between a value and the next in each dimension.

## Discussion

Pass `nil` to `dataLayout` to have `init(size:dataLayout:stride:)` return a shape with the default layout for the rank that’s equal to the count of `size`. The default layouts for each dimensionality are:

1D  
BNNS.DataLayout.vector

2D  
BNNS.DataLayout.matrixFirstMajor

3D  
BNNS.DataLayout.tensor3DFirstMajor

4D  
BNNS.DataLayout.tensor4DFirstMajor

5D  
BNNS.DataLayout.tensor5DFirstMajor

6D  
BNNS.DataLayout.tensor6DFirstMajor

7D  
BNNS.DataLayout.tensor7DFirstMajor

8D  
BNNS.DataLayout.tensor8DFirstMajor

This initializer interprets a stride value of `0` to mean that values are contiguous for that axis.

## See Also

### Creating a Shape

init(arrayLiteral: BNNS.Shape.ArrayLiteralElement...)

Returns a new shape with the specified size.

