

- MediaExtension
- METrackInfo
-  requiresFrameReordering 

Instance Property

# requiresFrameReordering

A Boolean value that indicates whether frame reordering occurs in the track.

macOS 14.0+

``` source
var requiresFrameReordering: Bool { get set }
```

## Discussion

The value is true if frame reordering occurs, otherwise false. This property is only valid for tracks with video media type and is false for other track types.

## See Also

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

