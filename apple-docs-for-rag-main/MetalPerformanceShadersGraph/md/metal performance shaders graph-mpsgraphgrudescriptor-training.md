

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  training 

Instance Property

# training

A parameter that enables the GRU layer to support training.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var training: Bool { get set }
```

## Discussion

If set to `YES` then the layer will produce training state tensor as a secondary output. Default value: `NO`.

