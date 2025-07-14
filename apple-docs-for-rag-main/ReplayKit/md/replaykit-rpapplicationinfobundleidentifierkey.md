

- ReplayKit
-  RPApplicationInfoBundleIdentifierKey 

Global Variable

# RPApplicationInfoBundleIdentifierKey

The key to retrieve the app’s bundle identifier from the user-information dictionary.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
let RPApplicationInfoBundleIdentifierKey: String
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

func processSampleBuffer(CMSampleBuffer, with: RPSampleBufferType)

Processes video and audio data as it becomes available during a live broadcast.

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

