

- Quartz
- QCCompositionParameterView
-  setCompositionRenderer(\_:) Deprecated

Instance Method

# setCompositionRenderer(\_:)

Sets the composition parameter view for editing the input parameters of the provided renderer object.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setCompositionRenderer(_ renderer: (any QCCompositionRenderer)!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`renderer`  

A `QCCompositionRenderer` object, either QCView, QCRenderer, or QCCompositionLayer. Pass `nil` to unset this renderer.

## Discussion

If the renderer is a QCView object, the view track the composition.

## See Also

### Getting and Setting the Renderer

func compositionRenderer() -> (any QCCompositionRenderer)!

Returns the renderer object associated with the composition parameter view.

Deprecated

