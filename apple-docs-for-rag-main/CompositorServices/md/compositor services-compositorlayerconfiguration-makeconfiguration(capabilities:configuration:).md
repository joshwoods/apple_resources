

- Compositor Services
- CompositorLayerConfiguration
-  makeConfiguration(capabilities:configuration:) 

Instance Method

# makeConfiguration(capabilities:configuration:)

Creates and returns a type that contains the rendering options for Compositor Services to use when configuring a layer.

CompositorServicesSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
func makeConfiguration(
    capabilities: LayerRenderer.Capabilities,
    configuration: inout LayerRenderer.Configuration
)
```

**Required**

## Parameters 

`capabilities`  

The supported capabilities of the current device. Use these values to validate any choices you apply to the `configuration` parameter.

`configuration`  

The default set of configuration options. Modify this type to specify the options you want to use during rendering.

## Mentioned in 

Drawing fully immersive content using Metal

## Discussion

In your implementation of this method, modify the `configuration` parameter to specify the Metal texture formats and layouts you want to use during rendering. Verify that your preferred choices are available by checking the supported options using the information in the `capabilities` parameter.

