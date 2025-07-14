

- Core ML
- MLModelConfiguration
-  preferredMetalDevice 

Instance Property

# preferredMetalDevice

The metal device you prefer this model use to make predictions (inference) and update the model.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var preferredMetalDevice: (any MTLDevice)? { get set }
```

## Discussion

If preferredMetalDevice is `nil`, the default value, Core ML chooses a metal device for you.

## See Also

### Configuring GPU Usage

var allowLowPrecisionAccumulationOnGPU: Bool

A Boolean value that determines whether to allow low-precision accumulation on a GPU.

