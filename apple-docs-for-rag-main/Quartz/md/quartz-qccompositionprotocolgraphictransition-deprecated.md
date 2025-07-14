

- Quartz
-  QCCompositionProtocolGraphicTransition Deprecated

Global Variable

# QCCompositionProtocolGraphicTransition

A composition that performs a transition between two images, using a transition time in range of `0` to `1`. A conforming composition must use the input keys QCCompositionInputSourceImageKey for the starting image and QCCompositionInputDestinationImageKey for the image to transition to. The composition can optionally use QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

macOS 10.4–10.15Deprecated

``` source
let QCCompositionProtocolGraphicTransition: String
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## See Also

### Constants

let QCCompositionAttributeBuiltInKey: String

The key for the composition origin.

Deprecated

let QCCompositionAttributeCategoryKey: String

A key representing a composition category.

Deprecated

let QCCompositionAttributeCopyrightKey: String

The key for composition copyright information. The associated value is an `NSString` object.

Deprecated

let QCCompositionAttributeDescriptionKey: String

The key for the composition description. The associated value is an `NSString` object.

Deprecated

let QCCompositionAttributeHasConsumersKey: String

The key for a composition that has consumer patches.

Deprecated

let QCCompositionAttributeIsTimeDependentKey: StringDeprecated

let QCCompositionAttributeNameKey: String

The key for the composition name. The associated value is an `NSString` object.

Deprecated

let QCCompositionCategoryDistortion: String

A composition that produces a distortion effect.

Deprecated

let QCCompositionCategoryStylize: String

A composition that produces a stylize effect.

Deprecated

let QCCompositionCategoryUtility: String

A utility composition.

Deprecated

let QCCompositionInputAudioPeakKey: String

A number input port whose key is `inputAudioPeak`. The value must be in the `[0,1]` range as a mono signal with no decay applied.

Deprecated

let QCCompositionInputAudioSpectrumKey: String

A structure input port whose key is `inputAudioSpectrum`. The structure must contain 16 values in the `[0,1]` range representing 16 spectrum bands of the mono signal from low to high frequencies with no decay applied.

Deprecated

let QCCompositionInputDestinationImageKey: String

An image input port whose key is `inputDestinationImage`.

Deprecated

let QCCompositionInputImageKey: String

An image input port whose key is `inputImage`.

Deprecated

let QCCompositionInputPaceKey: String

A number input port whose key is `inputPace`. The value must be in the `[0,1]` range.

