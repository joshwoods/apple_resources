

- Metal Performance Shaders Graph
- MPSGraphLSTMDescriptor
-  forgetGateLast 

Instance Property

# forgetGateLast

A parameter that controls the internal order of the LSTM gates.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
var forgetGateLast: Bool { get set }
```

## Discussion

If set to `YES` then the layer will use the gate-ordering `[ i, z, f, o ]` instead of default `[ i, f, z, o ]`. Default value: `NO`

