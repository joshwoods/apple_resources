

- Metal Performance Shaders Graph
- MPSGraph
-  bandPart(\_:numLowerTensor:numUpperTensor:name:) 

Instance Method

# bandPart(\_:numLowerTensor:numUpperTensor:name:)

Creates the band part operation and returns the result.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func bandPart(
    _ inputTensor: MPSGraphTensor,
    numLowerTensor: MPSGraphTensor,
    numUpperTensor: MPSGraphTensor,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`inputTensor`  

The source tensor to copy.

`numLowerTensor`  

Scalar Int32 tensor. The number of diagonals in the lower triangle to keep. If -1, keep all.

`numUpperTensor`  

Scalar Int32 tensor. The number of diagonals in the upper triangle to keep. If -1, keep all.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

See above discussion of bandPartWithTensor: numLower: numUpper: name:

