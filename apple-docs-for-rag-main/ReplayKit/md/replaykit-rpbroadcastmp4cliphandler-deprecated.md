

- ReplayKit
-  RPBroadcastMP4ClipHandler Deprecated

Class

# RPBroadcastMP4ClipHandler

An object that processes MP4 movie clips from ReplayKit.

iOS 10.0–11.0DeprecatediPadOS 10.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 10.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
class RPBroadcastMP4ClipHandler
```

Deprecated

Use RPBroadcastSampleHandler instead.

## Overview

Subclass this class to handle movie clips as ReplayKit records them during the broadcast. The system calls processMP4Clip(with:setupInfo:finished:) when a movie clip is available for processing.

## Topics

### Processing MP4 Movie Clips

func finishedProcessingMP4Clip(withUpdatedBroadcastConfiguration: RPBroadcastConfiguration?, error: (any Error)?)

Applies configuration update changes to the next MP4 movie clip.

func processMP4Clip(with: URL?, setupInfo: [String : NSObject]?, finished: Bool)

Processes MP4 movie clips for a live broadcast.

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

class RPBroadcastSampleHandler

An object that processes buffer objects as received from ReplayKit.

