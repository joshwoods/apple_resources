

- AVFoundation
- AVAssetWriter
-  directoryForTemporaryFiles 

Instance Property

# directoryForTemporaryFiles

A directory to contain temporary files that the export process generates.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var directoryForTemporaryFiles: URL? { get set }
```

## Discussion

In some configurations, such as performing multipass encoding, an asset writer may need to write temporary files. Use this property value to set the file-system location where it writes temporary files. The system deletes all temporary files after it finishes writing successfully, fails, or you cancel the writing session.

You can set this value after writing starts.

## See Also

### Configuring Output

var metadata: [AVMetadataItem]

An array of metadata items to write to the output file.

var shouldOptimizeForNetworkUse: Bool

A Boolean value that indicates whether to write the output file to make it more suitable for playback over a network.

