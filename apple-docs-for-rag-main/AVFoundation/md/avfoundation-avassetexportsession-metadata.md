

- AVFoundation
- AVAssetExportSession
-  metadata 

Instance Property

# metadata

The metadata an export session writes to the output container file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var metadata: [AVMetadataItem]? { get set }
```

## See Also

### Configuring Metadata

var metadataItemFilter: AVMetadataItemFilter?

An object the export session uses to filter the metadata items it transfers to the output asset.

