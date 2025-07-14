

- ReplayKit
- RPBroadcastMP4ClipHandler
-  finishedProcessingMP4Clip(withUpdatedBroadcastConfiguration:error:) Deprecated

Instance Method

# finishedProcessingMP4Clip(withUpdatedBroadcastConfiguration:error:)

Applies configuration update changes to the next MP4 movie clip.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func finishedProcessingMP4Clip(
    withUpdatedBroadcastConfiguration broadcastConfiguration: RPBroadcastConfiguration?,
    error: (any Error)?
)
```

Deprecated

No longer supported, use RPBroadcastSampleHandler instead.

## Parameters 

`broadcastConfiguration`  

Optional configuration update that is applied to the next MP4 movie clip.

`error`  

Indicates that an error occurred with the broadcast, and broadcasting is to stop.

## Discussion

Call this method when processing is complete. After this method is called, whether an error exists or not, the current MP4 movie clip is no longer available.

## See Also

### Processing MP4 Movie Clips

func processMP4Clip(with: URL?, setupInfo: [String : NSObject]?, finished: Bool)

Processes MP4 movie clips for a live broadcast.

Deprecated

