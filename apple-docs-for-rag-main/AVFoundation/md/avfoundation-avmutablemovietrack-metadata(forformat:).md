

- AVFoundation
- AVMutableMovieTrack
-  metadata(forFormat:) 

Instance Method

# metadata(forFormat:)

Returns metadata items that a track contains for the specified format.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
func metadata(forFormat format: AVMetadataFormat) -> [AVMetadataItem]
```

## Parameters 

`format`  

The format of the metadata items to retrieve.

## Return Value

An array of metadata items matching the specified format, or an empty array if none are found.

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata stored by the track.

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

