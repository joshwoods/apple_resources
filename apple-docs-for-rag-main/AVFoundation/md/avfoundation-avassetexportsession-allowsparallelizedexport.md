

- AVFoundation
- AVAssetExportSession
-  allowsParallelizedExport 

Instance Property

# allowsParallelizedExport

A Boolean value that indicates whether the session can parallelize its export operation.

macOS 14.0+

``` source
var allowsParallelizedExport: Bool { get set }
```

## Discussion

This value is true by default, which indicates that the export session is allowed to expedite its processing by using additional resources in parallel on select Mac systems. If parallelization isn’t achievable, export proceeds as normal.

Note

Parallelized exports reduce the amount of time it takes to export media, but require additional power consumption. If your app requires opting out of the default behavior, set this value to false.

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

var shouldOptimizeForNetworkUse: Bool

A Boolean value that indicates whether to optimize the movie for network use.

var canPerformMultiplePassesOverSourceMediaData: Bool

A Boolean value that indicates whether the export session can perform multiple passes over the source media to achieve better results.

var timeRange: CMTimeRange

The time range of the source asset to export.

var fileLengthLimit: Int64

The file length that the output of the session must not exceed.

var directoryForTemporaryFiles: URL?

A directory suitable to store temporary files that the export process generates.

