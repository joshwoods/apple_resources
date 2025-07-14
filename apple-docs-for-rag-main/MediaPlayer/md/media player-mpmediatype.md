

- Media Player
-  MPMediaType 

Structure

# MPMediaType

The properties for defining the type for a media item.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 9.0+visionOS 1.0+watchOS 5.0+

``` source
struct MPMediaType
```

## Overview

Media item types are possible values for the MPMediaItemPropertyMediaType property. A media item can have more than one media item type.

## Topics

### Constants

static var music: MPMediaType

The media item contains music.

static var podcast: MPMediaType

The media item contains a podcast.

static var audioBook: MPMediaType

The media item contains an audio book.

static var audioITunesU: MPMediaType

The media item contains an iTunes U audio lesson.

static var anyAudio: MPMediaType

The media item contains an unspecified type of audio content.

static var movie: MPMediaType

The media item contains a movie.

static var tvShow: MPMediaType

The media item contains a TV show.

static var videoPodcast: MPMediaType

The media item contains a video podcast.

static var musicVideo: MPMediaType

The media item contains a music video.

static var videoITunesU: MPMediaType

The media item contains an iTunes U video.

static var homeVideo: MPMediaType

The media item contains a home video.

static var anyVideo: MPMediaType

The media item contains an unspecified type of video content.

static var any: MPMediaType

The media item contains an unspecified type of media content.

### Initializers

init(rawValue: UInt)

Creates a new instance with the specified raw value.

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

### Media item types and keys

General media item property keys

System-defined properties for obtaining the metadata for a media item.

User-defined property keys

Properties for obtaining user-defined metadata for a media item.

