

- ActivityKit
- Activity
-  update(using:alertConfiguration:) Deprecated

Instance Method

# update(using:alertConfiguration:)

Updates the dynamic content of a Live Activity and alerts a person about the Live Activity update.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
func update(
    using contentState: Activity.ContentState,
    alertConfiguration: AlertConfiguration? = nil
) async
```

Deprecated

Use update(\_:alertConfiguration:) instead

## Parameters 

`contentState`  

The updated dynamic content for the Live Activity. The size of the encoded content can’t exceed 4KB in size.

`alertConfiguration`  

The alert configuration you use to configure how the system notifies a person about the updated content of the Live Activity.

## Discussion

The system ignores updates to a Live Activity that’s in the ActivityState.ended state.

## See Also

### Deprecated symbols

static func request(attributes: Attributes, contentState: Activity&lt;Attributes>.ContentState, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

Deprecated

var contentState: Activity&lt;Attributes>.ContentState

The dynamic content of a Live Activity.

Deprecated

func end(using: Activity&lt;Attributes>.ContentState?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

Deprecated

var contentStateUpdates: Activity&lt;Attributes>.ContentStateUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

Deprecated

struct ContentStateUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

Deprecated

