

- ActivityKit
- Activity
-  end(using:dismissalPolicy:) Deprecated

Instance Method

# end(using:dismissalPolicy:)

Ends an active Live Activity.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
func end(
    using contentState: Activity.ContentState? = nil,
    dismissalPolicy: ActivityUIDismissalPolicy = .default
) async
```

Deprecated

Use end(content:dismissalPolicy:) instead

## Parameters 

`contentState`  

The latest and final dynamic content for the Live Activity that ended. The size of the encoded content can’t exceed 4KB in size.

`dismissalPolicy`  

Describes how and when the system should dismiss a Live Activity and and remove it from the Lock Screen.

## Discussion

End an active Live Activity while your app is in the foreground or while it’s in the background — for example, by using Background Tasks.

Include updated data in the `contentState` parameter to ensure the Live Activity shows the latest and final content update after it ends. This is important because the Live Activity remains visible until the system or the person removes it.

## See Also

### Deprecated symbols

static func request(attributes: Attributes, contentState: Activity&lt;Attributes>.ContentState, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

Deprecated

var contentState: Activity&lt;Attributes>.ContentState

The dynamic content of a Live Activity.

Deprecated

func update(using: Activity&lt;Attributes>.ContentState, alertConfiguration: AlertConfiguration?) async

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

Deprecated

var contentStateUpdates: Activity&lt;Attributes>.ContentStateUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

Deprecated

struct ContentStateUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

Deprecated

