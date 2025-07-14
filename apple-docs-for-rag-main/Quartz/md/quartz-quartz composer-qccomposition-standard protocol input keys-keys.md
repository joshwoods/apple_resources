

- Quartz
- Quartz Composer
- QCComposition
-  Standard Protocol Input Keys 

API Collection

# Standard Protocol Input Keys

Input ports of a composition.

## Topics

### Constants

let QCCompositionInputImageKey: String

An image input port whose key is `inputImage`.

Deprecated

let QCCompositionInputSourceImageKey: String

An image input port whose key is `inputSourceImage`.

Deprecated

let QCCompositionInputDestinationImageKey: String

An image input port whose key is `inputDestinationImage`.

Deprecated

let QCCompositionInputRSSFeedURLKey: String

A string input port whose key is `inputRSSFeedURL`. This port must be passed an http or feed scheme URL.

Deprecated

let QCCompositionInputRSSArticleDurationKey: String

A number input port whose key is `inputRSSArticleDuration`. The value must be expressed in seconds.

Deprecated

let QCCompositionInputPreviewModeKey: String

A Boolean input port whose key is `inputPreviewMode`. When the value of this input port is set to `TRUE`, the composition that provides this port must be able to run in a low-quality mode that produces a preview of the composition.

Deprecated

let QCCompositionInputXKey: String

A number input port whose key is `inputX`. The value must be normalized to the image width with the origin on the left.

Deprecated

let QCCompositionInputYKey: String

A number input port whose key is `inputY`. The value must be normalized to the image height with the origin at the bottom.

Deprecated

let QCCompositionInputScreenImageKey: String

An image input port whose key is `inputScreenImage`.

Deprecated

let QCCompositionInputAudioPeakKey: String

A number input port whose key is `inputAudioPeak`. The value must be in the `[0,1]` range as a mono signal with no decay applied.

Deprecated

let QCCompositionInputAudioSpectrumKey: String

A structure input port whose key is `inputAudioSpectrum`. The structure must contain 16 values in the `[0,1]` range representing 16 spectrum bands of the mono signal from low to high frequencies with no decay applied.

Deprecated

let QCCompositionInputTrackPositionKey: String

A number input port whose key is `inputTrackPosition`. The value must be expressed in seconds.

Deprecated

let QCCompositionInputTrackInfoKey: String

A structure input port whose key is `inputTrackInfo`. The structure contains optional entries, such as “name”, “artist”, “album”, “duration”, “artwork”, and so on.

Deprecated

let QCCompositionInputTrackSignalKey: String

A Boolean input port whose key is `inputTrackSignal`.

Deprecated

let QCCompositionInputPrimaryColorKey: String

A color input port whose key is `inputPrimaryColor`.

Deprecated

let QCCompositionInputSecondaryColorKey: String

A color input port whose key is `inputSecondaryColor`.

Deprecated

let QCCompositionInputPaceKey: String

A number input port whose key is `inputPace`. The value must be in the `[0,1]` range.

## See Also

### Constants

Attribute Keys

Attributes of a composition.

Composition Categories

Categories for compositions.

Standard Protocol Output Keys

Output ports of a composition.

Standard Protocols

Protocols for a composition.

