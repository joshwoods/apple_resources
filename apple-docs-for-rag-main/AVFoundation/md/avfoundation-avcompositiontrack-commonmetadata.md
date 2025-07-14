

- AVFoundation
- AVCompositionTrack
-  commonMetadata 

Instance Property

# commonMetadata

An array of metadata items for all common metadata keys that have a value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var commonMetadata: [AVMetadataItem] { get }
```

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers that have a value.

var availableMetadataFormats: [AVMetadataFormat]

An array of metadata formats available for the track.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

