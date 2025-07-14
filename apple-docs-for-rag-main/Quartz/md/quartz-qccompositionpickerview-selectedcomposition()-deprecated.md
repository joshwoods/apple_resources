

- Quartz
- QCCompositionPickerView
-  selectedComposition() Deprecated

Instance Method

# selectedComposition()

Returns the composition that is currently selected in the composition picker view.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func selectedComposition() -> QCComposition!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A `QCComposition` object, or `nil` if a composition is not selected.

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

func setCompositionAspectRatio(NSSize)

Sets the aspect ratio used to display compositions in the composition picker view.

Deprecated

func compositionAspectRatio() -> NSSize

Retrieves the aspect ratio used to display compositions in the composition picker view.

Deprecated

func setSelectedComposition(QCComposition!)

Sets a composition as selected in the composition picker view.

Deprecated

