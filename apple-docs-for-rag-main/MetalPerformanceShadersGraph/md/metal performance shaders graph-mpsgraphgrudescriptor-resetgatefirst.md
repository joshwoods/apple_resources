

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  resetGateFirst 

Instance Property

# resetGateFirst

A parameter that controls the internal order of the GRU gates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var resetGateFirst: Bool { get set }
```

## Discussion

If set to `YES` then the layer will use the gate-ordering `[ r, z, o ]` instead of default `[ z, r, o ]`. Default value: `NO`.

