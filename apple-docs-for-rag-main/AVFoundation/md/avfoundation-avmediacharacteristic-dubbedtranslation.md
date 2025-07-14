

- AVFoundation
- AVMediaCharacteristic
-  dubbedTranslation 

Type Property

# dubbedTranslation

A media characteristic that indicates that a track or media selection option contains audio language or dialect translation of the original content.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let dubbedTranslation: AVMediaCharacteristic
```

## Discussion

The value of this characteristic is `public.translation.dubbed`.

For QuickTime movies and `.m4v` files, a media option has this characteristic only if the media’s author tags it that way.

## See Also

### Audible

static let audible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes audible content.

static let voiceOverTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language translation and verbal interpretation of spoken dialog.

static let enhancesSpeechIntelligibility: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes audio processed to enhance the intelligibility of speech.

static let describesMusicAndSoundForAccessibility: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes legible content in the language of its specified locale.

static let tactileMinimal: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes haptic content.

