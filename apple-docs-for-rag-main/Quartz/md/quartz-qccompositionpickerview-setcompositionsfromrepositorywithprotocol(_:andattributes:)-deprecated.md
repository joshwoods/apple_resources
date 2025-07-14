

- Quartz
- QCCompositionPickerView
-  setCompositionsFromRepositoryWithProtocol(\_:andAttributes:) Deprecated

Instance Method

# setCompositionsFromRepositoryWithProtocol(\_:andAttributes:)

Sets the compositions in the composition picker view to those that match the specified criteria.

macOS 10.4–10.15Deprecated

``` source
@MainActor
func setCompositionsFromRepositoryWithProtocol(
    _ protocol: String!,
    andAttributes attributes: [AnyHashable : Any]! = [:]
)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`protocol`  

The protocols that you want compositions shown in the picker view to conform to. You can pass any of these protocols: QCCompositionProtocolAnimation, QCCompositionProtocolImageProducer, QCCompositionProtocolImageFilter, QCCompositionProtocolImageCompositor, and QCCompositionProtocolScreenSaverRSS.

`attributes`  

A dictionary that contains the attributes, and their associated values, that you want compositions in the picker view to match. For example, you can pass: QCCompositionAttributeNameKey, QCCompositionAttributeDescriptionKey, QCCompositionAttributeCopyrightKey, and QCCompositionAttributeBuiltInKey. Pass `nil` if you don’t want to filter based on the attributes.

## See Also

### Managing the Composition Picker View

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

func selectedComposition() -> QCComposition!

Returns the composition that is currently selected in the composition picker view.

Deprecated

