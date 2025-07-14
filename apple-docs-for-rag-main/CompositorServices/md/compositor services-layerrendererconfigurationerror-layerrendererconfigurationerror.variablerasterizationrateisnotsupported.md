

- Compositor Services
- LayerRendererConfigurationError
-  LayerRendererConfigurationError.variableRasterizationRateIsNotSupported 

Case

# LayerRendererConfigurationError.variableRasterizationRateIsNotSupported

An error that indicates foveation is enabled but not supported.

visionOS 1.0+

``` source
case variableRasterizationRateIsNotSupported
```

## Discussion

Disable foveation in your layer’s configuration.

## See Also

### Getting the configuration errors

case layoutNotSupported

An error that indicates the configuration’s current layout value is invalid.

case missingConfiguration

An error that indicates the system didn’t find a default layer configuration.

case notEnoughFramesRequested

An error that indicates not enough frames are available for rendering.

case temporalAntiAliasingNotSupported

An error that occurs when you try to enable temporal anti-aliasing but the current configuration parameters don’t support it.

case tooManyFramesRequested

An error that indicates your app requested too many frames for rendering.

case unsupportedForwardDepthRange

An error that indicates the depth range values aren’t in reverse-z order.

case unsupportedNearPlaneDistance

An error that indicates the near plane of the client is closer than the minimum supported distance.

case unsupportedColorFormat

An error that indicates the system doesn’t support the specified color format choice.

case unsupportedColorUsage

An error that indicates the system doesn’t support the specified color usage option.

case unsupportedDepthFormat

An error that indicates the system doesn’t support the specified depth format choice.

case unsupportedDepthUsage

An error that indicates the system doesn’t support the specified depth usage choice.

