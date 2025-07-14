

- Metal Performance Shaders Graph
- MPSGraphPooling4DOpDescriptor
-  ceilMode 

Instance Property

# ceilMode

Affects how MPSGraph computes the output size: if set to `YES` then output size is computed by rounding up instead of down when dividing input size by stride.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var ceilMode: Bool { get set }
```

## Discussion

Default value: `NO`.

