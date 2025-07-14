

- ActivityKit
- Activity
-  contentStateUpdates Deprecated

Instance Property

# contentStateUpdates

An asynchronous sequence you use to observe changes to the dynamic content of a Live Activity.

iOS 16.1–16.2DeprecatediPadOS 16.1–16.2Deprecated

``` source
var contentStateUpdates: Activity.ContentStateUpdates { get }
```

Deprecated

Use contentUpdates instead

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

func end(using: Activity&lt;Attributes>.ContentState?, dismissalPolicy: ActivityUIDismissalPolicy) async

Ends an active Live Activity.

Deprecated

struct ContentStateUpdates

A structure that offers functionality to observe changes to the dynamic content of a Live Activity.

Deprecated

