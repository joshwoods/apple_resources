

- Compositor Services
- LayerRenderer
- LayerRenderer.Capabilities
-  LayerRenderer.Capabilities.SupportedLayoutsOptions 

Structure

# LayerRenderer.Capabilities.SupportedLayoutsOptions

Options you can use to filter the supported layouts for a layer.

visionOS 1.0+

``` source
struct SupportedLayoutsOptions
```

## Topics

### Getting the options

static let foveationEnabled: LayerRenderer.Capabilities.SupportedLayoutsOptions

An option to request a layout that supports foveated rendering.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- SetAlgebra

## See Also

### Getting the supported layouts

func supportedLayouts(options: LayerRenderer.Capabilities.SupportedLayoutsOptions) -> [LayerRenderer.Layout]

Returns an array of texture layouts that the layer supports.

