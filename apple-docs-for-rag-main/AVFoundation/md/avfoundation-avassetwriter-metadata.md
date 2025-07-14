

- AVFoundation
- AVAssetWriter
-  metadata 

Instance Property

# metadata

An array of metadata items to write to the output file.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var metadata: [AVMetadataItem] { get set }
```

## Discussion

You can’t modify this property value after writing starts.

## See Also

### Configuring Output

var shouldOptimizeForNetworkUse: Bool

A Boolean value that indicates whether to write the output file to make it more suitable for playback over a network.

var directoryForTemporaryFiles: URL?

A directory to contain temporary files that the export process generates.

