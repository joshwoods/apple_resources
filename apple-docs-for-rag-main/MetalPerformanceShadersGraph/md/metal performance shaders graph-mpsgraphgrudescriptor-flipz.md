

- Metal Performance Shaders Graph
- MPSGraphGRUDescriptor
-  flipZ 

Instance Property

# flipZ

A parameter that chooses between two variants for the final output computation.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var flipZ: Bool { get set }
```

## Discussion

If set to `YES` then the layer will compute the final value as `h[t] = z[t] h[t-1] + (1-z[t]) o[t]`. Otherwise it’s computed as `h[t] = (1-z[t]) h[t-1] + z[t] o[t]`. Default value: `NO`.

