

- Quartz
- QCCompositionParameterView
-  compositionRenderer() Deprecated

Instance Method

# compositionRenderer()

Returns the renderer object associated with the composition parameter view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func compositionRenderer() -> (any QCCompositionRenderer)!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A renderer object or `nil`, if the composition parameter view is not set to a renderer object.

## See Also

### Getting and Setting the Renderer

func setCompositionRenderer((any QCCompositionRenderer)!)

Sets the composition parameter view for editing the input parameters of the provided renderer object.

Deprecated

