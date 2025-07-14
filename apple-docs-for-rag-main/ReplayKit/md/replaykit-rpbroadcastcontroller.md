

- ReplayKit
-  RPBroadcastController 

Class

# RPBroadcastController

An object containing methods for starting and controlling a broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
class RPBroadcastController
```

## Topics

### Controlling the Broadcast

var broadcastURL: URL

A URL that redirects users to an ongoing or completed broadcast.

func startBroadcast(handler: ((any Error)?) -> Void)

Starts a broadcast.

func pauseBroadcast()

Pauses the current broadcast.

func resumeBroadcast()

Resumes a paused broadcast.

func finishBroadcast(handler: ((any Error)?) -> Void)

Stops the current broadcast.

var serviceInfo: [String : any NSCoding &amp; NSObjectProtocol]?

Information updated by the service during a broadcast.

### Retrieving Information About the Broadcast

var broadcastExtensionBundleID: String?

The bundle ID for the selected broadcast service.

Deprecated

var isBroadcasting: Bool

A Boolean value indicating whether the controller is broadcasting.

var isPaused: Bool

A Boolean value indicating whether the broadcast is paused.

### Getting the Delegate

var delegate: (any RPBroadcastControllerDelegate)?

The delegate for the broadcast controller.

protocol RPBroadcastControllerDelegate

The protocol you implement to respond to changes in a live broadcast.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Media Clip Processing

class RPBroadcastHandler

An object that sends messages to the broadcasting app.

class RPBroadcastSampleHandler

An object that processes buffer objects as received from ReplayKit.

class RPBroadcastMP4ClipHandler

An object that processes MP4 movie clips from ReplayKit.

Deprecated

