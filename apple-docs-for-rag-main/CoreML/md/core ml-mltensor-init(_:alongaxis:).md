

- Core ML
- MLTensor
-  init(\_:alongAxis:) 

Initializer

# init(\_:alongAxis:)

Creates a tensor by stacking the given tensors along the specified axis.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    _ elements: some Collection,
    alongAxis axis: Int = 0
)
```

## Parameters 

`axis`  

The axis along which to stack. Negative values wrap around.

