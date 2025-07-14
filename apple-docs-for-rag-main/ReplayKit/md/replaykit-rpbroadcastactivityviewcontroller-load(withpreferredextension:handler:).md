

- ReplayKit
- RPBroadcastActivityViewController
-  load(withPreferredExtension:handler:) 

Type Method

# load(withPreferredExtension:handler:)

Loads a broadcast activity view controller with a preferred extension.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class func load(
    withPreferredExtension preferredExtension: String?,
    handler: @escaping (RPBroadcastActivityViewController?, (any Error)?) -> Void
)
```

## Parameters 

`preferredExtension`  

The extension bundle identifier for the preferred broadcast extension service.

`handler`  

A block that is called after the view controller is loaded.

broadcastActivityViewController  
The `RPBroadcastActivityViewController` to be presented.

error  
If an error occurred, this parameter holds an object that explains the error. Otherwise, the value of this parameter is `nil`. See RPRecordingErrorCode for a list of error codes specific to ReplayKit.

## Discussion

Present the view controller using present(_:animated:completion:). Dismiss the view controller when the delegate’s broadcastActivityViewController(_:didFinishWith:error:) method is called.

Note

On the iPad, the default presentation style for view controllers is a popover. For an instance of `RPBroadcastActivityViewController` to present properly on iPad, insure the popover presentation controller’s sourceRect and sourceView are configured.

## See Also

### Presenting the Broadcast Activity UI

class func load(handler: (RPBroadcastActivityViewController?, (any Error)?) -> Void)

Loads a broadcast activity view controller.

