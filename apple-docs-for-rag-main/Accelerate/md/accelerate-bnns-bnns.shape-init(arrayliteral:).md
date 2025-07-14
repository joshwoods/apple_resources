

- Accelerate
- BNNS
- BNNS.Shape
-  init(arrayLiteral:) 

Initializer

# init(arrayLiteral:)

Returns a new shape with the specified size.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
init(arrayLiteral: BNNS.Shape.ArrayLiteralElement...)
```

## Parameters 

`arrayLiteral`  

An array that specifies the number of values in each dimension.

## Discussion

This initializer returns a shape with the default layout for the rank that’s equal to the count of `arrayLiteral`. The default layouts for each dimensionality are:

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

## See Also

### Creating a Shape

init([Int], dataLayout: BNNS.DataLayout?, stride: [Int]?)

Returns a new shape with the specified size, data layout, and stride.

