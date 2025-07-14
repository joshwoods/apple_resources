

- Compositor Services
- LayerRenderer
- LayerRenderer.Capabilities
-  supportedLayouts(options:) 

Instance Method

# supportedLayouts(options:)

Returns an array of texture layouts that the layer supports.

visionOS 1.0+

``` source
func supportedLayouts(options: LayerRenderer.Capabilities.SupportedLayoutsOptions) -> [LayerRenderer.Layout]
```

## Parameters 

`options`  

Specific options you want the layouts to support. The function returns only layouts that support the specified options.

## Return Value

An array of supported layouts. If the layer doesn’t support any layouts with the specified options, this function returns an empty array.

## Discussion

Call this function to determine which texture layouts you can use for your content.

## See Also

### Getting the supported layouts

struct SupportedLayoutsOptions

Options you can use to filter the supported layouts for a layer.

