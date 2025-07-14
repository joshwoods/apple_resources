

- ReplayKit
- RPBroadcastController
-  finishBroadcast(handler:) 

Instance Method

# finishBroadcast(handler:)

Stops the current broadcast.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 11.0+tvOS 10.0+visionOS 1.0+

``` source
func finishBroadcast(handler: @escaping ((any Error)?) -> Void)
```

## Parameters 

`handler`  

A block that is called after the broadcast has finished.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## Discussion

Use this method when the user is finished with a broadcast. To temporarily pause a broadcast, use pauseBroadcast().

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

var serviceInfo: [String : any NSCoding &amp; NSObjectProtocol]?

Information updated by the service during a broadcast.

