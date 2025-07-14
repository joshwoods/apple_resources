

- Core ML
- MLModelConfiguration
-  allowLowPrecisionAccumulationOnGPU 

Instance Property

# allowLowPrecisionAccumulationOnGPU

A Boolean value that determines whether to allow low-precision accumulation on a GPU.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var allowLowPrecisionAccumulationOnGPU: Bool { get set }
```

## See Also

### Configuring GPU Usage

var preferredMetalDevice: (any MTLDevice)?

The metal device you prefer this model use to make predictions (inference) and update the model.

