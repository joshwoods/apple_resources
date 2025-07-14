

- ReplayKit
- RPBroadcastSampleHandler
-  broadcastFinished() 

Instance Method

# broadcastFinished()

Perform any required actions after a live broadcast is finished.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func broadcastFinished()
```

## Discussion

ReplayKit calls this method when the the broadcasting app calls its finishBroadcast(handler:) method.

## See Also

### Handling Sample Buffer Clips

func broadcastStarted(withSetupInfo: [String : NSObject]?)

Perform any required actions after starting a live broadcast.

func broadcastPaused()

Perform any required actions after a live broadcast is paused.

func broadcastResumed()

Perform any required actions after a live broadcast is resumed.

func broadcastAnnotated(withApplicationInfo: [AnyHashable : Any])

Perform any required actions after starting a live broadcast.

let RPApplicationInfoBundleIdentifierKey: String

The key to retrieve the app’s bundle identifier from the user-information dictionary.

func processSampleBuffer(CMSampleBuffer, with: RPSampleBufferType)

Processes video and audio data as it becomes available during a live broadcast.

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

