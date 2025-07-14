

- Quartz
- Quartz Composer
-  Quartz Composer Constants 

API Collection

# Quartz Composer Constants

## Topics

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

let QCCompositionInputPreviewModeKey: String

A Boolean input port whose key is `inputPreviewMode`. When the value of this input port is set to `TRUE`, the composition that provides this port must be able to run in a low-quality mode that produces a preview of the composition.

Deprecated

let QCCompositionInputPrimaryColorKey: String

A color input port whose key is `inputPrimaryColor`.

Deprecated

let QCCompositionInputRSSArticleDurationKey: String

A number input port whose key is `inputRSSArticleDuration`. The value must be expressed in seconds.

Deprecated

let QCCompositionInputRSSFeedURLKey: String

A string input port whose key is `inputRSSFeedURL`. This port must be passed an http or feed scheme URL.

Deprecated

let QCCompositionInputScreenImageKey: String

An image input port whose key is `inputScreenImage`.

Deprecated

let QCCompositionInputSecondaryColorKey: String

A color input port whose key is `inputSecondaryColor`.

Deprecated

let QCCompositionInputSourceImageKey: String

An image input port whose key is `inputSourceImage`.

Deprecated

let QCCompositionInputTrackInfoKey: String

A structure input port whose key is `inputTrackInfo`. The structure contains optional entries, such as “name”, “artist”, “album”, “duration”, “artwork”, and so on.

Deprecated

let QCCompositionInputTrackPositionKey: String

A number input port whose key is `inputTrackPosition`. The value must be expressed in seconds.

Deprecated

let QCCompositionInputTrackSignalKey: String

A Boolean input port whose key is `inputTrackSignal`.

Deprecated

let QCCompositionInputXKey: String

A number input port whose key is `inputX`. The value must be normalized to the image width with the origin on the left.

Deprecated

let QCCompositionInputYKey: String

A number input port whose key is `inputY`. The value must be normalized to the image height with the origin at the bottom.

Deprecated

let QCCompositionOutputImageKey: String

An image output port whose key is `outputImage`.

Deprecated

let QCCompositionOutputWebPageURLKey: String

A string output port whose key is `outputWebPageURL`.

Deprecated

let QCCompositionProtocolGraphicAnimation: String

A composition that renders a generic graphical animation. It has the option to use QCCompositionInputPrimaryColorKey for the primary color of the animation, QCCompositionInputSecondaryColorKey for the secondary color of the animation, QCCompositionInputPaceKey for the global pace of the animation, and QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolGraphicTransition: String

A composition that performs a transition between two images, using a transition time in range of `0` to `1`. A conforming composition must use the input keys QCCompositionInputSourceImageKey for the starting image and QCCompositionInputDestinationImageKey for the image to transition to. The composition can optionally use QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolImageFilter: String

A composition that applies an effect to a source image. A conforming composition must use the input key QCCompositionInputImageKey for the source image and QCCompositionOutputImageKey for the output image. The composition can optionally use QCCompositionInputXKey to specify the X position of the center point of the effect, QCCompositionInputYKey to specify the Y position of the center point of the effect, andQCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes.

Deprecated

let QCCompositionProtocolMusicVisualizer: String

A composition that acts as a visualizer for music. A conforming composition must use the input key QCCompositionInputAudioPeakKey for the instantaneous audio peak and the QCCompositionInputAudioSpectrumKey for the instantaneous audio spectrum. It can optionally use the QCCompositionInputTrackInfoKey to indicate it receives information about the current track and the QCCompositionInputTrackSignalKey to indicate the start of a new track.

Deprecated

let QCCompositionProtocolRSSVisualizer: String

A composition that acts as a visualizer for an RSS feed. A conforming composition must use the input key QCCompositionInputRSSFeedURLKey for the URL to use for the RSS feed. It can optionally use QCCompositionInputRSSArticleDurationKey to specify the duration of each feed article.

Deprecated

let QCCompositionProtocolScreenSaver: String

A composition that can be used as a screen saver. The composition has the option to use QCCompositionInputScreenImageKey for a screenshot image of the screen that the screen saver runs on, QCCompositionInputPreviewModeKey to indicate if the animation should run in lower-quality for preview purposes, and QCCompositionOutputWebPageURLKey for a URL to open in the default web browser when screen saver exits (only allowed if screen saver password is disabled).

Deprecated

let QCPlugInAttributeCategoriesKey: StringDeprecated

let QCPlugInAttributeCopyrightKey: StringDeprecated

let QCPlugInAttributeDescriptionKey: String

The key for the custom patch description.

Deprecated

let QCPlugInAttributeExamplesKey: StringDeprecated

let QCPlugInAttributeNameKey: String

The key for the custom patch name.

Deprecated

let QCPlugInExecutionArgumentEventKey: String

The current event.

Deprecated

let QCPlugInExecutionArgumentMouseLocationKey: String

The current location of the mouse (as an `NSPoint` object stored in an `NSValue` object) in normalized coordinates relative to the OpenGL context viewport (\[0,1\]x\[0,1\] with the origin (`0,0`) at the lower-left corner).

Deprecated

let QCPlugInPixelFormatARGB8: String

An ARGB8 format. The alpha component is stored in the most significant bits of each pixel. Each pixel component is 8 bits. For best performance, use this format on PowerPC-based Macintosh computers, as it represents of the order of the data in memory.

Deprecated

let QCPlugInPixelFormatBGRA8: String

A BGRA8 format. The alpha component is stored in the least significant bits of each pixel. Each pixel component is 8 bits. For best performance, use this format on Intel-PC-based Macintosh computers, as it represents of the order of the data in memory.

Deprecated

let QCPlugInPixelFormatI8: String

An I8 format. Intensity information is represented as an 8-bit value.

Deprecated

let QCPlugInPixelFormatIf: String

An If format. Intensity information is represented as a floating-point value.

Deprecated

let QCPlugInPixelFormatRGBAf: String

An RGBAf format. Pixel components are represented as floating-point values.

Deprecated

let QCPortAttributeDefaultValueKey: String

The key for the port default value. You can use this key only for value ports (Boolean, Index, Number, Color and String).

Deprecated

let QCPortAttributeMaximumValueKey: String

The key for the port maximum value.

Deprecated

let QCPortAttributeMenuItemsKey: String

The key for the menu items.

Deprecated

let QCPortAttributeMinimumValueKey: String

The key for the port minimum value.

Deprecated

let QCPortAttributeNameKey: String

The key for the port name.

Deprecated

let QCPortAttributeTypeKey: String

The key for the port type. The associated value can be of any of the following constants: QCPortTypeBoolean, QCPortTypeIndex, QCPortTypeNumber, QCPortTypeString, QCPortTypeColor, QCPortTypeImage, or QCPortTypeStructure.

Deprecated

let QCPortTypeBoolean: String

The port type for a Boolean value.

Deprecated

let QCPortTypeColor: String

The port type for a color value.

Deprecated

let QCPortTypeImage: String

The port type for an image.

Deprecated

let QCPortTypeIndex: String

The port type for an index value.

Deprecated

let QCPortTypeNumber: String

The port type for a number value.

Deprecated

let QCPortTypeString: String

The port type for a string. The associated value can be an NSString object or any object that responds to the `-stringValue` or `-description` methods.

Deprecated

let QCPortTypeStructure: String

The port type for a collection.

Deprecated

let QCRendererEventKey: String

A key for a renderer event.

Deprecated

let QCRendererMouseLocationKey: String

A key for the mouse location.

Deprecated

var kQCPlugInExecutionModeConsumer: QCPlugInExecutionMode

A consumer execution mode. The custom patch always executes assuming the value of its Enable input port is `true`. (The Enable port is automatically added by the system.)

var kQCPlugInExecutionModeProcessor: QCPlugInExecutionMode

A processor execution mode. The custom patch executes whenever its inputs change or if the time change (assuming it’s time-dependent).

var kQCPlugInExecutionModeProvider: QCPlugInExecutionMode

A provider execution mode. The custom patch executes on demand—that is, whenever data is requested of it, but at most once per frame.

var kQCPlugInTimeModeIdle: QCPlugInTimeMode

An idle time dependency. The custom patch does not depend on time but needs the system to execute it periodically. For example if the custom patch connects to a piece of hardware, to ensure that it pulls data from the hardware, you would set the custom patch time dependency to idle time mode. This time mode is typically used with providers.\]\]

var kQCPlugInTimeModeNone: QCPlugInTimeMode

No time dependency. The custom patch does not depend on time at all. (It does not use the `time` parameter of the `execute:atTime:withArguments:` method.)

var kQCPlugInTimeModeTimeBase: QCPlugInTimeMode

A time base dependency. The custom patch does depend on time explicitly and has a time base defined by the system. (It uses the `time` parameter of the `execute:atTime:withArguments:` method.)

## See Also

### Reference

Quartz Data Types

Quartz Constants

Quartz Enumerations

Quartz Composer Enumerations

