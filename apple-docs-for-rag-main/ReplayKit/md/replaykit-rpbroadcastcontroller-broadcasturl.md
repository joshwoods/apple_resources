

- ReplayKit
- RPBroadcastController
-  broadcastURL 

Instance Property

# broadcastURL

A URL that redirects users to an ongoing or completed broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
var broadcastURL: URL { get }
```

## See Also

### Controlling the Broadcast

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

