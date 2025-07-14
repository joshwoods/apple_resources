

- ReplayKit
- RPBroadcastMP4ClipHandler
-  processMP4Clip(with:setupInfo:finished:) Deprecated

Instance Method

# processMP4Clip(with:setupInfo:finished:)

Processes MP4 movie clips for a live broadcast.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func processMP4Clip(
    with mp4ClipURL: URL?,
    setupInfo: [String : NSObject]?,
    finished: Bool
)
```

Deprecated

No longer supported, use RPBroadcastSampleHandler instead.

## Parameters 

`mp4ClipURL`  

URL that points to the location of the movie clip. This parameter is `nil` when an error occurs.

`setupInfo`  

Dictionary that is supplied by the UI extension and contains setup information required for processing. The values contained in the dictionary are defined by the extension developer.

`finished`  

Boolean value indicating that the app has requested the broadcast to end. Set to true to end the broadcast.

## See Also

### Processing MP4 Movie Clips

func finishedProcessingMP4Clip(withUpdatedBroadcastConfiguration: RPBroadcastConfiguration?, error: (any Error)?)

Applies configuration update changes to the next MP4 movie clip.

Deprecated

