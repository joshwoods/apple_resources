

- ActivityKit
-  ActivityAuthorizationError 

Enumeration

# ActivityAuthorizationError

An error that indicates why the request to start a Live Activity failed.

iOS 16.1+iPadOS 16.1+

``` source
enum ActivityAuthorizationError
```

## Topics

### Error codes

case attributesTooLarge

The provided Live Activity attributes exceeded the maximum size of 4KB.

case denied

A person deactivated Live Activities in Settings.

case globalMaximumExceeded

The device reached the maximum number of ongoing Live Activities.

case malformedActivityIdentifier

The provided activity identifier is malformed.

case missingProcessIdentifier

The process that tried to start the Live Activity is missing a process identifier.

case persistenceFailure

The system couldn’t persist the Live Activity.

case reconnectNotPermitted

The process that tried to recreate the Live Activity is not the process that originally created the Live Activity.

case targetMaximumExceeded

The app has already started the maximum number of concurrent Live Activities.

case unentitled

The app doesn’t have the required entitlement to start a Live Activity.

case unsupported

The device doesn’t support Live Activities.

case unsupportedTarget

The app doesn’t have the required entitlement to start a Live Activities.

case visibility

The app tried to start the Live Activity while it was in the background.

### Getting error information

var failureReason: String?

A string that describes the error that occurred.

var recoverySuggestion: String?

A localized message that describes how to recover from the error.

### Protocol confirmation

var errorCode: Int

An integer value that represents the error code.

static var errorDomain: String

The domain for errors that can happen when starting a Live Activity.

### Operators

static func == (ActivityAuthorizationError, ActivityAuthorizationError) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomNSError Implementations

Equatable Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Copyable
- CustomNSError
- Equatable
- Error
- Hashable
- LocalizedError
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

struct ActivityContent

A structure that describes the state and configuration of a Live Activity.

typealias ContentState

The type alias for the structure that describes the dynamic content of a Live Activity.

struct PushType

The structure that offers constants you use to configure a Live Activity to receive updates through ActivityKit push notifications.

static func request(attributes: Attributes, content: ActivityContent&lt;Activity&lt;Attributes>.ContentState>, pushType: PushType?, style: ActivityStyle) throws -> Activity&lt;Attributes>

