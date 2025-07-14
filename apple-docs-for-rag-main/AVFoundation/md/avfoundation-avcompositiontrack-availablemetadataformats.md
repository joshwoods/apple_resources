

- AVFoundation
- AVCompositionTrack
-  availableMetadataFormats 

Instance Property

# availableMetadataFormats

An array of metadata formats available for the track.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var availableMetadataFormats: [AVMetadataFormat] { get }
```

## See Also

### Accessing Metadata

var metadata: [AVMetadataItem]

An array of metadata items for all metadata identifiers that have a value.

var commonMetadata: [AVMetadataItem]

An array of metadata items for all common metadata keys that have a value.

func metadata(forFormat: AVMetadataFormat) -> [AVMetadataItem]

Returns metadata items that a track contains for the specified format.

