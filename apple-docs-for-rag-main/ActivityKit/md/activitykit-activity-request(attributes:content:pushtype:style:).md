

- ActivityKit
- Activity
-  request(attributes:content:pushType:style:) 

Type Method

# request(attributes:content:pushType:style:)

iOS 18.0+iPadOS 18.0+

``` source
static func request(
    attributes: Attributes,
    content: ActivityContent.ContentState>,
    pushType: PushType? = nil,
    style: ActivityStyle
) throws -> Activity
```

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

typealias ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

struct PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

enum ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

