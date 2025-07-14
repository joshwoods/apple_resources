

- Media Accessibility
-  Captions 

API Collection

# Captions

Coordinate the presentation of closed-captioned data for your app’s media files.

## Overview

People can create custom styles for caption appearance in Accessibility settings. The Media Accessibility framework provides access to these user-captioning settings.

In macOS, choose System Settings \> Accessibility \> Captions to access these options.

When a person creates a custom caption style, the settings affect attributes, such as caption color, font, and language.

By choosing custom styles for media text, people are requesting improved legibility. The Media Accessibility functions let you to tailor the user experience of your media content. You must be able to influence the caption-rendering process at time of delivery for the following functions to be useful. Retrieving a person’s preferences and dynamically rendering the captions for maximum readability provides the best user experience.

## Topics

### General settings

let kMACaptionAppearanceSettingsChangedNotification: CFString

A notification that occurs when any user-defined caption settings change.

func MACaptionAppearanceDidDisplayCaptions(CFArray)

Informs accessibility clients when captions display onscreen.

func MACaptionAppearanceCopyPreferredCaptioningMediaCharacteristics(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferences for captioning sounds.

func MACaptionAppearanceGetDisplayType(MACaptionAppearanceDomain) -> MACaptionAppearanceDisplayType

Returns the preferred type of captions to display.

func MACaptionAppearanceSetDisplayType(MACaptionAppearanceDomain, MACaptionAppearanceDisplayType)

Sets the preference for the type of caption.

### Language settings

func MACaptionAppearanceAddSelectedLanguage(MACaptionAppearanceDomain, CFString) -> Bool

Adds a preference for caption language to the stack of languages.

func MACaptionAppearanceCopySelectedLanguages(MACaptionAppearanceDomain) -> Unmanaged&lt;CFArray>

Returns the preferred caption languages.

### Text settings

func MACaptionAppearanceCopyFontDescriptorForStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?, MACaptionAppearanceFontStyle) -> Unmanaged&lt;CTFontDescriptor>

Returns the preferred font for the specified style of type.

func MACaptionAppearanceCopyForegroundColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for text color.

func MACaptionAppearanceGetForegroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for text opacity.

func MACaptionAppearanceGetRelativeCharacterSize(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for font scaling.

func MACaptionAppearanceGetTextEdgeStyle(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> MACaptionAppearanceTextEdgeStyle

Returns the preference for text edge style.

### Text highlight settings

func MACaptionAppearanceCopyBackgroundColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for the text highlight color.

func MACaptionAppearanceGetBackgroundOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for the text highlight opacity.

### Caption window settings

func MACaptionAppearanceCopyWindowColor(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> Unmanaged&lt;CGColor>

Returns the preference for the caption window’s color.

func MACaptionAppearanceGetWindowOpacity(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the preference for the overlay’s opacity.

func MACaptionAppearanceGetWindowRoundedCornerRadius(MACaptionAppearanceDomain, UnsafeMutablePointer&lt;MACaptionAppearanceBehavior>?) -> CGFloat

Returns the radius of the caption window’s corners.

### Image captioning settings

func MAImageCaptioningCopyCaption(CFURL, UnsafeMutablePointer&lt;CFError?>?) -> CFString?

Returns an accessibility caption from an image’s metadata.

func MAImageCaptioningSetCaption(CFURL, CFString?, UnsafeMutablePointer&lt;CFError?>?) -> Bool

Sets the accessibility caption for an image’s metadata.

func MAImageCaptioningCopyMetadataTagPath() -> CFString

Returns the metadata tag path.

### Audible media selection settings

let kMAAudibleMediaSettingsChangedNotification: CFString

A notification that occurs when any user-defined audible media settings change.

func MAAudibleMediaCopyPreferredCharacteristics() -> Unmanaged&lt;CFArray>

Returns the preference for audible media characteristics.

let MAMediaCharacteristicDescribesVideoForAccessibility: CFString

A media characteristic that indicates that a track or media selection option includes audible content that describes a video for accessibility.

let MAMediaCharacteristicDescribesMusicAndSoundForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that describes music and sound other than spoken dialog.

let MAMediaCharacteristicTranscribesSpokenDialogForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that transcribes spoken dialog and identifies the speakers.

### Constants

enum MACaptionAppearanceDomain

A value that specifies which domain to retrieve a preference setting from.

enum MACaptionAppearanceDisplayType

A value that specifies the type of captions to display.

enum MACaptionAppearanceBehavior

A value that indicates the preferred behavior for a preference setting.

enum MACaptionAppearanceFontStyle

A value that specifies a font style.

enum MACaptionAppearanceTextEdgeStyle

A value that specifies a style for the outside of the text.

## See Also

### Features

Flashing lights

Detect, mitigate, and inform people about flashing lights in media content.

Music Haptics

Play haptic tracks along with known music tracks.

