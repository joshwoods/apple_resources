

- Core ML
- MLTensor
-  .\

Operator

# .\

Computes element-wise less comparison between two tensors.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
static func . MLTensor
```

## Return Value

A Boolean tensor where each element is true if the left hand side tensor is less than the corresponding element of the right hand side, and false otherwise.

## Discussion

Shapes must be broadcastable, where the broadcasted shape becomes the shape of the output.

