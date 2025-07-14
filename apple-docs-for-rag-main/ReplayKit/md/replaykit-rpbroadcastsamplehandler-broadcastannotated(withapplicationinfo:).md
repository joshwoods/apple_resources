

- ReplayKit
- RPBroadcastSampleHandler
-  broadcastAnnotated(withApplicationInfo:) 

Instance Method

# broadcastAnnotated(withApplicationInfo:)

Perform any required actions after starting a live broadcast.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 11.0+visionOS 1.0+

``` source
func broadcastAnnotated(withApplicationInfo applicationInfo: [AnyHashable : Any])
```

## Parameters 

`applicationInfo`  

A dictionary containing information about the first application opened or used buring the broadcast.

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

let RPApplicationInfoBundleIdentifierKey: String

The key to retrieve the app’s bundle identifier from the user-information dictionary.

func processSampleBuffer(CMSampleBuffer, with: RPSampleBufferType)

Processes video and audio data as it becomes available during a live broadcast.

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

