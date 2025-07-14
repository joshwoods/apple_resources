

- Quartz
- QCCompositionPickerView
-  setCompositionAspectRatio(\_:) Deprecated

Instance Method

# setCompositionAspectRatio(\_:)

Sets the aspect ratio used to display compositions in the composition picker view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setCompositionAspectRatio(_ ratio: NSSize)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`ratio`  

An aspect ratio.

## See Also

### Managing the Composition Picker View

func setCompositionsFromRepositoryWithProtocol(String!, andAttributes: [AnyHashable : Any]!)

Sets the compositions in the composition picker view to those that match the specified criteria.

Deprecated

func compositions() -> [Any]!

Returns the list of compositions that are currently in the composition picker view.

Deprecated

func setAllowsEmptySelection(Bool)

Sets whether to allow an empty selection in the composition picker view.

Deprecated

func allowsEmptySelection() -> Bool

Retrieves the empty-selection state of the composition picker view.

Deprecated

func compositionAspectRatio() -> NSSize

Retrieves the aspect ratio used to display compositions in the composition picker view.

Deprecated

func setSelectedComposition(QCComposition!)

Sets a composition as selected in the composition picker view.

Deprecated

func selectedComposition() -> QCComposition!

Returns the composition that is currently selected in the composition picker view.

Deprecated

