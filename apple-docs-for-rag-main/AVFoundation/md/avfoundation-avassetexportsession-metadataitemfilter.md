

- AVFoundation
- AVAssetExportSession
-  metadataItemFilter 

Instance Property

# metadataItemFilter

An object the export session uses to filter the metadata items it transfers to the output asset.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var metadataItemFilter: AVMetadataItemFilter? { get set }
```

## Discussion

The default value is `nil`.

## See Also

### Configuring Metadata

var metadata: [AVMetadataItem]?

The metadata an export session writes to the output container file.

