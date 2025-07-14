

- Quartz
- Quartz Composer
- QCComposition
-  Standard Protocols 

API Collection

# Standard Protocols

Protocols for a composition.

## Topics

### Constants

let QCCompositionProtocolGraphicAnimation: String

A composition that renders a generic graphical animation. It has the option to use QCCompositionInputPrimaryColorKey for the primary color of the animation, QCCompositionInputSecondaryColorKey for the secondary color of the animation, QCCompositionInputPaceKey for the global pace of the animation, and QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolGraphicTransition: String

A composition that performs a transition between two images, using a transition time in range of `0` to `1`. A conforming composition must use the input keys QCCompositionInputSourceImageKey for the starting image and QCCompositionInputDestinationImageKey for the image to transition to. The composition can optionally use QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolImageFilter: String

A composition that applies an effect to a source image. A conforming composition must use the input key QCCompositionInputImageKey for the source image and QCCompositionOutputImageKey for the output image. The composition can optionally use QCCompositionInputXKey to specify the X position of the center point of the effect, QCCompositionInputYKey to specify the Y position of the center point of the effect, andQCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolScreenSaver: String

A composition that can be used as a screen saver. The composition has the option to use QCCompositionInputScreenImageKey for a screenshot image of the screen that the screen saver runs on, QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes, and QCCompositionOutputWebPageURLKey for a URL to open in the default web browser when screen saver exits (only allowed if screen saver password is disabled).

Deprecated

let QCCompositionProtocolRSSVisualizer: String

A composition that acts as a visualizer for an RSS feed. A conforming composition must use the input key QCCompositionInputRSSFeedURLKey for the URL to use for the RSS feed. It can optionally use QCCompositionInputRSSArticleDurationKey to specify the duration of each feed article.

Deprecated

let QCCompositionProtocolMusicVisualizer: String

A composition that acts as a visualizer for music. A conforming composition must use the input key QCCompositionInputAudioPeakKey for the instantaneous audio peak and the QCCompositionInputAudioSpectrumKey for the instantaneous audio spectrum. It can optionally use the QCCompositionInputTrackInfoKey to indicate it receives information about the current track and the QCCompositionInputTrackSignalKey to indicate the start of a new track.

Deprecated

## See Also

### Constants

Attribute Keys

Attributes of a composition.

Composition Categories

Categories for compositions.

Standard Protocol Input Keys

Input ports of a composition.

Standard Protocol Output Keys

Output ports of a composition.

