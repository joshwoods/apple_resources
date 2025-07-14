

- AVFoundation
- AVAssetExportSession
-  timeRange 

Instance Property

# timeRange

The time range of the source asset to export.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var timeRange: CMTimeRange { get set }
```

## See Also

### Configuring Output

var outputURL: URL?

A URL where an asset export session writes its output.

Deprecated

var outputFileType: AVFileType?

The file type of the output an asset export session writes.

Deprecated

var supportedFileTypes: [AVFileType]

An array containing the types of files the session can write.

var allowsParallelizedExport: Bool

A Boolean value that indicates whether the session can parallelize its export operation.

var shouldOptimizeForNetworkUse: Bool

A Boolean value that indicates whether to optimize the movie for network use.

var canPerformMultiplePassesOverSourceMediaData: Bool

A Boolean value that indicates whether the export session can perform multiple passes over the source media to achieve better results.

var fileLengthLimit: Int64

The file length that the output of the session must not exceed.

var directoryForTemporaryFiles: URL?

A directory suitable to store temporary files that the export process generates.

