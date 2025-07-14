

- ReplayKit
-  RPVideoSampleOrientationKey 

Global Variable

# RPVideoSampleOrientationKey

The sample attachment key that describes the video orientation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 11.0+tvOS 11.0+visionOS 1.0+

``` source
let RPVideoSampleOrientationKey: String
```

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

func processSampleBuffer(CMSampleBuffer, with: RPSampleBufferType)

Processes video and audio data as it becomes available during a live broadcast.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

