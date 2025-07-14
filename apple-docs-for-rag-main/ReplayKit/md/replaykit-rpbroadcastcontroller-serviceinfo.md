

- ReplayKit
- RPBroadcastController
-  serviceInfo 

Instance Property

# serviceInfo

Information updated by the service during a broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
var serviceInfo: [String : any NSCoding & NSObjectProtocol]? { get }
```

## Discussion

The keys and values for the dictionary are defined by the broadcast service and updated through the updateServiceInfo(_:) function. This property is KVO observable.

## See Also

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

