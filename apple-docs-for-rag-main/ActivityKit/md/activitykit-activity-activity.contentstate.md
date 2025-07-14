

- ActivityKit
- Activity
-  Activity.ContentState 

Type Alias

# Activity.ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

iOS 16.1+iPadOS 16.1+

``` source
typealias ContentState = Attributes.ContentState
```

## Mentioned in 

Displaying live data with Live Activities

Starting and updating Live Activities with ActivityKit push notifications

## See Also

### Starting a Live Activity

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

let attributes: Attributes

A set of attributes that describe a Live Activity and its content.

protocol ActivityAttributes

The protocol you implement to describe the content of a Live Activity.

enum ActivityStyle

var content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>

The dynamic content of a Live Activity.

struct ActivityContent

A structure that describes the state and configuration of a Live Activity.

struct PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

enum ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

