

- Media Accessibility
-  MAMediaCharacteristicDescribesVideoForAccessibility 

Global Variable

# MAMediaCharacteristicDescribesVideoForAccessibility

A media characteristic that indicates that a track or media selection option includes audible content that describes a video for accessibility.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 17.0+visionOS 1.0+

``` source
let MAMediaCharacteristicDescribesVideoForAccessibility: CFString
```

## See Also

### Audible media selection settings

let kMAAudibleMediaSettingsChangedNotification: CFString

A notification that occurs when any user-defined audible media settings change.

func MAAudibleMediaCopyPreferredCharacteristics() -> Unmanaged&lt;CFArray>

Returns the preference for audible media characteristics.

let MAMediaCharacteristicDescribesMusicAndSoundForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that describes music and sound other than spoken dialog.

let MAMediaCharacteristicTranscribesSpokenDialogForAccessibility: CFString

A media characteristic that indicates that a track includes legible content in the language of its specified locale that transcribes spoken dialog and identifies the speakers.

