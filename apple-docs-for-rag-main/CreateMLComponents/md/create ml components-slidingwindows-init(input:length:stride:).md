

- Create ML Components
- SlidingWindows
-  init(input:length:stride:) 

Initializer

# init(input:length:stride:)

Creates a sliding windows sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
init(
    input: MLShapedArray,
    length: Int,
    stride: Int = 1
) throws
```

## Parameters 

`input`  

A shaped array having two dimensions.

`length`  

The number of samples in each window. Must be positive.

`stride`  

The number of samples between windows. Must be positive. Defaults to 1.

