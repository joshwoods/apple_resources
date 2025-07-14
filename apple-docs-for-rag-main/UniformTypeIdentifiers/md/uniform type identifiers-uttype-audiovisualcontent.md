

- Uniform Type Identifiers
- UTType
-  audiovisualContent 

Type Property

# audiovisualContent

A base type that represents data that contains video content that may or may not also include audio.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var audiovisualContent: UTType { get }
```

## Discussion

The identifier for this type is `public.audiovisual-content`.

This type conforms to UTTypeContent and UTTypeData.

## See Also

### Image, audio, and video base types

static var image: UTType

A base type that represents image data.

static var audio: UTType

A type that represents audio that doesn’t contain video.

static var movie: UTType

A base type representing media formats that may contain both video and audio.

static var video: UTType

A type that represents video that doesn’t contain audio.

