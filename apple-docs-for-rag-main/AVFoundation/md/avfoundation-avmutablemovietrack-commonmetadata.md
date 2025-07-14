

- AVFoundation
- AVMutableMovieTrack
-  commonMetadata 

Instance Property

# commonMetadata

An array of metadata items for all common metadata keys that have a value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var commonMetadata: [AVMetadataItem] { get }
```

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata stored by the track.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

