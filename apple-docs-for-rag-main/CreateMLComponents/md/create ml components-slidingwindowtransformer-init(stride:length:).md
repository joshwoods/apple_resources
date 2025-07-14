

- Create ML Components
- SlidingWindowTransformer
-  init(stride:length:) 

Initializer

# init(stride:length:)

Creates a window temporal transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    stride: Int,
    length: Int
)
```

## Parameters 

`stride`  

The number of frames between the start of two consecutive windows. Must be greater than 0.

`length`  

The length of a window in number of frames. Must be greater than 0.

## See Also

### Creating a transformer

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

