

- ReplayKit
- RPBroadcastActivityViewController
-  load(handler:) 

Type Method

# load(handler:)

Loads a broadcast activity view controller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
class func load(handler: @escaping (RPBroadcastActivityViewController?, (any Error)?) -> Void)
```

## Parameters 

`handler`  

A block that is called after the view controller is loaded.

`broadcastActivityViewController`  
The `RPBroadcastActivityViewController` to be presented.

`error`  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## Discussion

Present the view controller using present(_:animated:completion:). Dismiss the view controller when the delegate’s broadcastActivityViewController(_:didFinishWith:error:) method is called.

Note

On the iPad, the default presentation style for view controllers is a popover. For an instance of `RPBroadcastActivityViewController` to present properly on iPad, insure the popover presentation controller’s sourceRect and sourceView are configured.

## See Also

### Presenting the Broadcast Activity UI

class func load(withPreferredExtension: String?, handler: (RPBroadcastActivityViewController?, (any Error)?) -> Void)

Loads a broadcast activity view controller with a preferred extension.

