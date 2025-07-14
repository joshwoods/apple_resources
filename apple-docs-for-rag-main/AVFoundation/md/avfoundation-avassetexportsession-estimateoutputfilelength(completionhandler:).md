

- AVFoundation
- AVAssetExportSession
-  estimateOutputFileLength(completionHandler:) 

Instance Method

# estimateOutputFileLength(completionHandler:)

Starts estimating the output file length of the export while considering the asset, preset, and time range configuration of the export session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func estimateOutputFileLength(completionHandler handler: @escaping (Int64, (any Error)?) -> Void)
```

``` source
var estimatedOutputFileLengthInBytes: Int64 { get async throws }
```

## Parameters 

`handler`  

A callback the system invokes when it finishes its estimation. It passes the callback the following parameters:

`estimatedOutputFileLength`  
The system’s estimation of the output file length.

`error`  
An error object if the request fails; otherwise, `nil`.

## See Also

### Estimating File Length and Duration

var estimatedOutputFileLength: Int64

The estimated length of the exported file, in bytes.

Deprecated

