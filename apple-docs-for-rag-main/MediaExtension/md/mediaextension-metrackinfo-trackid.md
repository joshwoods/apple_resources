

- MediaExtension
- METrackInfo
-  trackID 

Instance Property

# trackID

An integer that identifies the track within the media asset.

macOS 14.0+

``` source
var trackID: CMPersistentTrackID { get }
```

## Discussion

The track ID uniquely identifes the track within a MEFormatReader object. Track IDs must be unique within a media asset but don’t need to be unique across assets. If a media format doesn’t have a native concept of track IDs, track IDs can start from `1`. However, track ID `0` is a reserved value to indicate an invalid track ID.

## See Also

### Inspecting track information

var mediaType: CMMediaType

The media type of the track.

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

