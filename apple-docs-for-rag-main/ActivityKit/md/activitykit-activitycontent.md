

- ActivityKit
-  ActivityContent 

Structure

# ActivityContent

A structure that describes the state and configuration of a Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
struct ActivityContent where State : Decodable, State : Encodable, State : Hashable
```

## Mentioned in 

Displaying live data with Live Activities

## Topics

### Describing a Live Activity

init(state: State, staleDate: Date?, relevanceScore: Double)

Creates the object that describes the state and configuration of a Live Activity.

let state: State

The current state of a Live Activity in its life cycle.

let staleDate: Date?

The date when the system considers the Live Activity to be out of date.

let relevanceScore: Double

A score you assign that determines the order in which your Live Activities appear when you start several Live Activities for your app.

### Default Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- Sendable

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

typealias ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

struct PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

enum ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

