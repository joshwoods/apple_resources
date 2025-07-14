

- AVFoundation
- AVMediaCharacteristic
-  describesMusicAndSoundForAccessibility 

Type Property

# describesMusicAndSoundForAccessibility

A media characteristic that indicates that a track or media selection option includes legible content in the language of its specified locale.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let describesMusicAndSoundForAccessibility: AVMediaCharacteristic
```

## Discussion

Legible media options may include transcriptions of spoken dialog and descriptions of music and sound effects.

The value of this characteristic is `public.accessibility.describes-music-and-sound`.

For QuickTime movies and `.m4v` files, a media option has this characteristic only if the media’s author tags it that way.

## See Also

### Audible

static let audible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes audible content.

static let dubbedTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains audio language or dialect translation of the original content.

static let voiceOverTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language translation and verbal interpretation of spoken dialog.

static let enhancesSpeechIntelligibility: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes audio processed to enhance the intelligibility of speech.

static let tactileMinimal: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes haptic content.

