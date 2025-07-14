

- Media Accessibility
-  kMAAudibleMediaSettingsChangedNotification 

Global Variable

# kMAAudibleMediaSettingsChangedNotification

A notification that occurs when any user-defined audible media settings change.

iOS 17.0+iPadOS 17.0+Mac Catalyst 13.0+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
let kMAAudibleMediaSettingsChangedNotification: CFString
```

## See Also

### Audible media selection settings

func MAAudibleMediaCopyPreferredCharacteristics() -> Unmanaged&lt;CFArray>

Returns the preference for audible media characteristics.

let MAMediaCharacteristicDescribesVideoForAccessibility: CFString

A media characteristic that indicates that a track or media selection option includes audible content that describes a video for accessibility.

let MAMediaCharacteristicDescribesMusicAndSoundForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that describes music and sound other than spoken dialog.

let MAMediaCharacteristicTranscribesSpokenDialogForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that transcribes spoken dialog and identifies the speakers.

