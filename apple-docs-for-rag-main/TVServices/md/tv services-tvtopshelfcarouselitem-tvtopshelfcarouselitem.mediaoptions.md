

- TV Services
- TVTopShelfCarouselItem
-  TVTopShelfCarouselItem.MediaOptions 

Structure

# TVTopShelfCarouselItem.MediaOptions

Constants indicating the item’s audio and video capabilities.

tvOS 13.0+

``` source
struct MediaOptions
```

## Topics

### Media Options

static var videoResolutionHD: TVTopShelfCarouselItem.MediaOptions

High-definition video resolution.

static var videoResolution4K: TVTopShelfCarouselItem.MediaOptions

Ultra-high-definition 4K video resolution.

static var videoColorSpaceHDR: TVTopShelfCarouselItem.MediaOptions

High-dynamic-range video.

static var videoColorSpaceDolbyVision: TVTopShelfCarouselItem.MediaOptions

Dolby Vision video.

static var audioDolbyAtmos: TVTopShelfCarouselItem.MediaOptions

Audio content with Dolby Atmos.

static var audioTranscriptionClosedCaptioning: TVTopShelfCarouselItem.MediaOptions

Audio content with closed captioning.

static var audioTranscriptionSDH: TVTopShelfCarouselItem.MediaOptions

Audio content with subtitles for people who are deaf or hard of hearing.

static var audioDescription: TVTopShelfCarouselItem.MediaOptions

Audio content with audio descriptions.

### Initializers

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Adding Media Badges

var mediaOptions: TVTopShelfCarouselItem.MediaOptions

Information about the media format and presentation options.

