

- AVFoundation
- AVMediaCharacteristic
-  describesVideoForAccessibility 

Type Property

# describesVideoForAccessibility

A media characteristic that indicates the media includes audible content that describes the visual portion of the presentation.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
static let describesVideoForAccessibility: AVMediaCharacteristic
```

## Discussion

It’s possible for a legible media option to include both transcriptions of spoken dialog and descriptions of music and sound effects.

The value of this characteristic is `public.accessibility.describes-video`.

For QuickTime movies and `.m4v` files, a media option has this characteristic only if the media’s author tags it that way.

## See Also

### Legible

static let legible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes legible content.

static let easyToRead: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option provides legible content that’s edited for easy reading.

static let containsOnlyForcedSubtitles: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option presents only forced subtitles.

static let languageTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language or dialect translation of the original content.

static let transcribesSpokenDialogForAccessibility: AVMediaCharacteristic

A media characteristic that indicates that a media selection option includes legible content that transcribes spoken dialog.

