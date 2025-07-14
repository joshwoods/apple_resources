

- Metal Performance Shaders Graph
- MPSGraph
-  bandPart(\_:numLower:numUpper:name:) 

Instance Method

# bandPart(\_:numLower:numUpper:name:)

Computes the band part of an input tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func bandPart(
    _ inputTensor: MPSGraphTensor,
    numLower: Int,
    numUpper: Int,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`inputTensor`  

Input tensor

`numLower`  

The number of diagonals in the lower triangle to keep. If -1, the framework returns all sub diagnols.

`numUpper`  

The number of diagonals in the upper triangle to keep. If -1, the framework returns all super diagnols.

`name`  

Name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

This operation copies a diagonal band of values from input tensor to a result tensor of the same size. A coordinate `[..., i, j]` is in the band if

```
(numLower 

The values outside of the band are set to 0.

