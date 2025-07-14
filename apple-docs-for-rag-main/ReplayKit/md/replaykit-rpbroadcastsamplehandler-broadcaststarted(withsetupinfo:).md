

- ReplayKit
- RPBroadcastSampleHandler
-  broadcastStarted(withSetupInfo:) 

Instance Method

# broadcastStarted(withSetupInfo:)

Perform any required actions after starting a live broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func broadcastStarted(withSetupInfo setupInfo: [String : NSObject]?)
```

## Parameters 

`setupInfo`  

A dictionary supplied by the ReplayKit UI extension that contains any required setup information.

## Discussion

ReplayKit calls this method when the the broadcasting app calls its startBroadcast(handler:) method.

## See Also

### Handling Sample Buffer Clips

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

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

