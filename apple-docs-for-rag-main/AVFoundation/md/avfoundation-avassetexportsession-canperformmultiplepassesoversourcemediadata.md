

- AVFoundation
- AVAssetExportSession
-  canPerformMultiplePassesOverSourceMediaData 

Instance Property

# canPerformMultiplePassesOverSourceMediaData

A Boolean value that indicates whether the export session can perform multiple passes over the source media to achieve better results.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
var canPerformMultiplePassesOverSourceMediaData: Bool { get set }
```

## Discussion

When the value for this property is true, the export session can produce higher quality results at the expense of longer export times. Setting this property to true may also require the export session to write temporary data to disk during the export. To control the location of temporary data, use the property directoryForTemporaryFiles.

The default value is false. Not all export session configurations can benefit from performing multiple passes over the source media. In these cases, setting this property to true has no effect.

You can’t set this property after the export starts.

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

var timeRange: CMTimeRange

The time range of the source asset to export.

var fileLengthLimit: Int64

The file length that the output of the session must not exceed.

var directoryForTemporaryFiles: URL?

A directory suitable to store temporary files that the export process generates.

