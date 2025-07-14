

- MediaExtension
-  METrackInfo 

Class

# METrackInfo

An object that includes track properties parsed from the media asset.

macOS 14.0+

``` source
class METrackInfo
```

## Topics

### Inspecting track information

var mediaType: CMMediaType

The media type of the track.

var trackID: CMPersistentTrackID

An integer that identifies the track within the media asset.

var isEnabled: Bool

A Boolean value that indicates whether the track is enabled by default.

var naturalTimescale: CMTimeScale

The natural timescale of the track.

var extendedLanguageTag: String?

A string that indicates the language tag associated with the track, as an IETF BCP 47 (RFC 4646) language identifier.

var naturalSize: CGSize

Indicates the natural dimensions of the media data referenced by the track.

var preferredTransform: CGAffineTransform

Indicates the preferred affine display transform of the track media for visual display.

var nominalFrameRate: Float32

The frame rate of the track in frames per second, as a 32-bit floating point number.

var requiresFrameReordering: Bool

A Boolean value that indicates whether frame reordering occurs in the track.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Track readers

protocol METrackReader

A protocol that defines the information to provide about a track within a media asset.

