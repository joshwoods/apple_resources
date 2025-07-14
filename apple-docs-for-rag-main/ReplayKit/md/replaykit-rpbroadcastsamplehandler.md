

- ReplayKit
-  RPBroadcastSampleHandler 

Class

# RPBroadcastSampleHandler

An object that processes buffer objects as received from ReplayKit.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
class RPBroadcastSampleHandler
```

## Overview

To handle CMSampleBuffer objects as captured by ReplayKit, you subclass `RPBroadcastSampleHandler`. You enable this mode of handling by setting `RPBroadcastProcessMode` in the extension’s ``` I``nfo.plist ``` file to `RPBroadcastProcessModeSampleBuffer`.

In your subclass, implement the processSampleBuffer(_:with:) method to handle video and audio buffers, as well as the broadcastStarted(withSetupInfo:), broadcastFinished(), broadcastPaused(), and broadcastResumed() methods to handle starting and stopping the broadcast.

ReplayKit invokes methods in your `RPBroadcastSampleHandler` subclass in a serial fashion. After invoking one method, ReplayKit won’t invoke another method until the first method returns. That means it’s safe for your implementations to update their stored state without the use of locks or synchronization to provide thread safety.

## Topics

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

let RPVideoSampleOrientationKey: String

The sample attachment key that describes the video orientation.

func finishBroadcastWithError(any Error)

Stops the broadcast and passes an error back to the broadcasting app.

## Relationships

### Inherits From

- RPBroadcastHandler

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSExtensionRequestHandling
- NSObjectProtocol

## See Also

### Media Clip Processing

class RPBroadcastController

An object containing methods for starting and controlling a broadcast.

class RPBroadcastHandler

An object that sends messages to the broadcasting app.

class RPBroadcastMP4ClipHandler

An object that processes MP4 movie clips from ReplayKit.

Deprecated

