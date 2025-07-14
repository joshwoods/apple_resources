

- AVFoundation
-  AVMediaCharacteristic 

Structure

# AVMediaCharacteristic

A structure that defines media data characteristics.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVMediaCharacteristic
```

## Discussion

QuickTime Movie and MPEG-4 video files may contain tracks that provide tagged media characteristics to indicate a purpose, trait, or feature of the track’s media. For example, an audio track that mixes original program content with additional narrative descriptions of visual action may have the media characteristic `public.accessibility.describes-video` to distinguish it from other audio tracks stored in the same file that don’t contain additional narrative.

You inspect the tagged media characteristics of a track as shown below:

```
NSArray *userDataItems = [myAVAssetTrack metadataForFormat:AVMetadataFormatQuickTimeUserData];
NSArray *trackTaggedMediaCharacteristics = [AVMetadataItem metadataItemsFromArray: userDataItems
        withKey: AVMetadataQuickTimeUserDataKeyTaggedCharacteristic
        keySpace: AVMetadataKeySpaceQuickTimeUserData];
for (AVMetadataItem *metadataItem in trackTaggedMediaCharacteristics) {
     NSString *thisTrackMediaCharacteristic = [metadataItem stringValue];
}
```

You write tagged media characteristics to files of type mov and m4v by using an instance of AVAssetWriter. You indicate tagged characteristics for a track by setting metadata on its associated asset writer input as shown below:

```
AVMutableMetadataItem *myTaggedMediaCharacteristic = [[AVMutableMetadataItem alloc] init];
[myTaggedMediaCharacteristic setKey:AVMetadataQuickTimeUserDataKeyTaggedCharacteristic];
[myTaggedMediaCharacteristic setKeySpace:AVMetadataKeySpaceQuickTimeUserData];
[myTaggedMediaCharacteristic setValue:aMeaningfulCharacteristicAsNSString];
[myMutableArrayOfMetadata addObject:myTaggedMediaCharacteristic];
[myAssetWriterInput setMetadata:myMutableArrayOfMetadata];
```

## Topics

### Visual

static let visual: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes visual content.

static let containsAlphaChannel: AVMediaCharacteristic

A media characteristic that indicates that a track contains an alpha channel.

static let containsHDRVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains HDR video.

static let frameBased: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes frame-based content.

static let usesWideGamutColorSpace: AVMediaCharacteristic

A media characteristic that indicates that a track uses a wide-gamut color space.

static let containsStereoMultiviewVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains stereoscopic video captured in a multiview compression format.

static let carriesVideoStereoMetadata: AVMediaCharacteristic

A media characteristic that indicates that the stereoscopic video track carries additional information related to the stereoscopic video.

static let indicatesHorizontalFieldOfView: AVMediaCharacteristic

A media characteristic that indicates the video track carries information related to the horizontal field of view.

### Audible

static let audible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes audible content.

static let dubbedTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains audio language or dialect translation of the original content.

static let voiceOverTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language translation and verbal interpretation of spoken dialog.

static let enhancesSpeechIntelligibility: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes audio processed to enhance the intelligibility of speech.

static let describesMusicAndSoundForAccessibility: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes legible content in the language of its specified locale.

static let tactileMinimal: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes haptic content.

### Legible

static let legible: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes legible content.

static let easyToRead: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option provides legible content that’s edited for easy reading.

static let describesVideoForAccessibility: AVMediaCharacteristic

A media characteristic that indicates the media includes audible content that describes the visual portion of the presentation.

static let containsOnlyForcedSubtitles: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option presents only forced subtitles.

static let languageTranslation: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains a language or dialect translation of the original content.

static let transcribesSpokenDialogForAccessibility: AVMediaCharacteristic

A media characteristic that indicates that a media selection option includes legible content that transcribes spoken dialog.

### Content

static let isOriginalContent: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option contains original content.

static let isMainProgramContent: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes content its author indicates is essential to the asset’s presentation.

static let isAuxiliaryContent: AVMediaCharacteristic

A media characteristic that indicates a track or media selection option includes content its author indicates is auxiliary to the asset’s presentation.

### Initializers

init(String)

Creates a media characteristic.

init(rawValue: String)

Creates a media characteristic with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Media types

struct AVMediaType

An identifier for various media types.

