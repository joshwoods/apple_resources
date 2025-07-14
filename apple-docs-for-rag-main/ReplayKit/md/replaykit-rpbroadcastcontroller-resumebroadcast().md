

- ReplayKit
- RPBroadcastController
-  resumeBroadcast() 

Instance Method

# resumeBroadcast()

Resumes a paused broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func resumeBroadcast()
```

## See Also

### Controlling the Broadcast

var broadcastURL: URL

A URL that redirects users to an ongoing or completed broadcast.

func startBroadcast(handler: ((any Error)?) -> Void)

Starts a broadcast.

func pauseBroadcast()

Pauses the current broadcast.

func finishBroadcast(handler: ((any Error)?) -> Void)

Stops the current broadcast.

var serviceInfo: [String : any NSCoding &amp; NSObjectProtocol]?

Information updated by the service during a broadcast.

