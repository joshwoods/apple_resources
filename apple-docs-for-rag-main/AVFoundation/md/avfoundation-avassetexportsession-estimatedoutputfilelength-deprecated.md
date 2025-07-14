

- AVFoundation
- AVAssetExportSession
-  estimatedOutputFileLength Deprecated

Instance Property

# estimatedOutputFileLength

The estimated length of the exported file, in bytes.

iOS 5.0–18.0DeprecatediPadOS 5.0–18.0DeprecatedMac Catalyst 13.1–18.0DeprecatedmacOS 10.9–15.0DeprecatedtvOS 5.0–18.0Deprecated

``` source
var estimatedOutputFileLength: Int64 { get }
```

Deprecated

Use estimateOutputFileLengthWithCompletionHandler: instead

## See Also

### Estimating File Length and Duration

func estimateOutputFileLength(completionHandler: (Int64, (any Error)?) -> Void)

Starts estimating the output file length of the export while considering the asset, preset, and time range configuration of the export session.

