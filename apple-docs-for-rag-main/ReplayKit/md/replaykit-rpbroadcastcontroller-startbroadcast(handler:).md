

- ReplayKit
- RPBroadcastController
-  startBroadcast(handler:) 

Instance Method

# startBroadcast(handler:)

Starts a broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func startBroadcast(handler: @escaping ((any Error)?) -> Void)
```

## Parameters 

`handler`  

A block that is called after a broadcast has started.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## See Also

### Controlling the Broadcast

var broadcastURL: URL

A URL that redirects users to an ongoing or completed broadcast.

func pauseBroadcast()

Pauses the current broadcast.

func resumeBroadcast()

Resumes a paused broadcast.

func finishBroadcast(handler: ((any Error)?) -> Void)

Stops the current broadcast.

var serviceInfo: [String : any NSCoding &amp; NSObjectProtocol]?

Information updated by the service during a broadcast.

