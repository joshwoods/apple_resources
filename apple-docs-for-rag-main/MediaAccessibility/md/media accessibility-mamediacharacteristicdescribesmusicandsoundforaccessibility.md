

- Media Accessibility
-  MAMediaCharacteristicDescribesMusicAndSoundForAccessibility 

Global Variable

# MAMediaCharacteristicDescribesMusicAndSoundForAccessibility

A media characteristic that indicates that a track includes legible content in the language of its specified locale that describes music and sound other than spoken dialog.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 17.0+visionOS 1.0+

``` source
let MAMediaCharacteristicDescribesMusicAndSoundForAccessibility: CFString
```

## See Also

### Audible media selection settings

let kMAAudibleMediaSettingsChangedNotification: CFString

A notification that occurs when any user-defined audible media settings change.

func MAAudibleMediaCopyPreferredCharacteristics() -> Unmanaged&lt;CFArray>

Returns the preference for audible media characteristics.

let MAMediaCharacteristicDescribesVideoForAccessibility: CFString

A media characteristic that indicates that a track or media selection option includes audible content that describes a video for accessibility.

let MAMediaCharacteristicTranscribesSpokenDialogForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that transcribes spoken dialog and identifies the speakers.

