

- AVFoundation
- AVMediaCharacteristic
-  containsOnlyForcedSubtitles 

Type Property

# containsOnlyForcedSubtitles

A media characteristic that indicates that a track or media selection option presents only forced subtitles.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let containsOnlyForcedSubtitles: AVMediaCharacteristic
```

## Discussion

The value of this characteristic is `public.subtitles.forced-only`.

The system infers this characteristic from the format description of the associated track.

## See Also

### Legible

static let legible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes legible content.

static let easyToRead: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option provides legible content that’s edited for easy reading.

static let describesVideoForAccessibility: AVMediaCharacteristic

A media characteristic that indicates the media includes audible content that describes the visual portion of the presentation.

static let languageTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language or dialect translation of the original content.

static let transcribesSpokenDialogForAccessibility: AVMediaCharacteristic

A media characteristic that indicates that a media selection option includes legible content that transcribes spoken dialog.

