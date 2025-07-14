

- Uniform Type Identifiers
- UTType
-  movie 

Type Property

# movie

A base type representing media formats that may contain both video and audio.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var movie: UTType { get }
```

## Discussion

This type corresponds to what users would label a “movie”.

The identifier for this type is `public.movie`.

This type conforms to UTTypeAudiovisualContent.

## See Also

### Image, audio, and video base types

static var image: UTType

A base type that represents image data.

static var audio: UTType

A type that represents audio that doesn’t contain video.

static var audiovisualContent: UTType

A base type that represents data that contains video content that may or may not also include audio.

static var video: UTType

A type that represents video that doesn’t contain audio.

