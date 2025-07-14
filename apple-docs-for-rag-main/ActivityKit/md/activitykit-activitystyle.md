

- ActivityKit
-  ActivityStyle 

Enumeration

# ActivityStyle

iOS 16.1+iPadOS 16.1+

``` source
enum ActivityStyle
```

## Topics

### Style

case standard

case transient

### Operators

static func == (ActivityStyle, ActivityStyle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Starting a Live Activity

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?) throws -> Activity&lt;Attributes>

Requests and starts a Live Activity.

let attributes: Attributes

A set of attributes that describe a Live Activity and its content.

protocol ActivityAttributes

The protocol you implement to describe the content of a Live Activity.

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

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

