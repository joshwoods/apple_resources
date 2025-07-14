

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  reverse 

Instance Property

# reverse

A parameter that defines the time direction of the input sequence.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var reverse: Bool { get set }
```

## Discussion

If set to `YES` then the input sequence is passed in reverse time order to the layer. Note: Ignored when `bidirectional = YES`. Default value: `NO`.

