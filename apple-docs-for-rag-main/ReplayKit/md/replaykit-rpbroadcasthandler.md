

- ReplayKit
-  RPBroadcastHandler 

Class

# RPBroadcastHandler

An object that sends messages to the broadcasting app.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
class RPBroadcastHandler
```

## Topics

### Updating Current Broadcast Information

func updateServiceInfo([String : any NSCoding &amp; NSObjectProtocol])

Sends information about the current broadcast to the broadcasting app.

func updateBroadcast(URL)

Sends the current broadcast URL to the broadcast controller.

## Relationships

### Inherits From

- NSObject

### Inherited By

- RPBroadcastMP4ClipHandler
- RPBroadcastSampleHandler

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

class RPBroadcastSampleHandler

An object that processes buffer objects as received from ReplayKit.

class RPBroadcastMP4ClipHandler

An object that processes MP4 movie clips from ReplayKit.

Deprecated

