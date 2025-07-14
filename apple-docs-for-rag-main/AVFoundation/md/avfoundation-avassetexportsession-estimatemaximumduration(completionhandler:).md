

- AVFoundation
- AVAssetExportSession
-  estimateMaximumDuration(completionHandler:) 

Instance Method

# estimateMaximumDuration(completionHandler:)

Starts estimating the maximum duration of the export while considering the asset, preset, and time range configuration of the export session.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func estimateMaximumDuration(completionHandler handler: @escaping (CMTime, (any Error)?) -> Void)
```

``` source
var estimatedMaximumDuration: CMTime { get async throws }
```

## Parameters 

`handler`  

A callback the system invokes when it finishes its estimation. It passes the callback the following parameters:

`estimatedMaximumDuration`  
The system’s estimation of the maximum duration.

`error`  
An optional error object that indicates if an error occurred during processing.

## See Also

### Estimating Duration

var maxDuration: CMTime

Provides an estimate of the maximum duration of the exported media.

Deprecated

