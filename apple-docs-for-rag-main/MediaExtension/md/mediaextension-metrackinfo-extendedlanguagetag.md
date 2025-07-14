

- MediaExtension
- METrackInfo
-  extendedLanguageTag 

Instance Property

# extendedLanguageTag

A string that indicates the language tag associated with the track, as an IETF BCP 47 (RFC 4646) language identifier.

macOS 14.0+

``` source
var extendedLanguageTag: String? { get set }
```

## Discussion

`MediaToolbox` uses this property to group similar language tracks together or to match audio and caption tracks. Set this value to `nil` if the track doesn’t have a language tag.

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

var naturalSize: CGSize

Indicates the natural dimensions of the media data referenced by the track.

var preferredTransform: CGAffineTransform

Indicates the preferred affine display transform of the track media for visual display.

var nominalFrameRate: Float32

The frame rate of the track in frames per second, as a 32-bit floating point number.

var requiresFrameReordering: Bool

A Boolean value that indicates whether frame reordering occurs in the track.

