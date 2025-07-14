

- ReplayKit
- RPBroadcastSampleHandler
-  processSampleBuffer(\_:with:) 

Instance Method

# processSampleBuffer(\_:with:)

Processes video and audio data as it becomes available during a live broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func processSampleBuffer(
    _ sampleBuffer: CMSampleBuffer,
    with sampleBufferType: RPSampleBufferType
)
```

## Parameters 

`sampleBuffer`  

A CMSampleBuffer object containing either audio or video data.

`sampleBufferType`  

An RPSampleBufferType identifying the media type of the recorded sample.

## Discussion

This method handles buffers of all sample buffer types throughout each broadcast. If no audio is available — for example, if the microphone isn’t capturing input — ReplayKit provides audio buffers whose samples represent continuous silence.

ReplayKit provides sample buffers sequentially. After invoking this method with a sample buffer, ReplayKit won’t invoke the method again for any sample buffer type until the current invocation returns.

The sample buffer passed to this method is available only until the method returns. You shouldn’t keep a reference to the sample buffer after the method returns.

## See Also

### Handling Sample Buffer Clips

func broadcastStarted(withSetupInfo: [String : NSObject]?)

Perform any required actions after starting a live broadcast.

func broadcastPaused()

Perform any required actions after a live broadcast is paused.

func broadcastResumed()

Perform any required actions after a live broadcast is resumed.

func broadcastFinished()

Perform any required actions after a live broadcast is finished.

func broadcastAnnotated(withApplicationInfo: [AnyHashable : Any])

Perform any required actions after starting a live broadcast.

let RPApplicationInfoBundleIdentifierKey: String

The key to retrieve the app’s bundle identifier from the user-information dictionary.

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

