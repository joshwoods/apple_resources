

- ActivityKit
-  ActivityState 

Enumeration

# ActivityState

The enum that describes the state of a Live Activity in its life cycle.

iOS 16.1+iPadOS 16.1+

``` source
enum ActivityState
```

## Mentioned in 

Displaying live data with Live Activities

## Topics

### Live Activity states

case active

The Live Activity is active, visible, and can receive content updates.

case dismissed

The Live Activity ended and is no longer visible because a person or the system removed it.

case stale

The Live Activity content is out of date and needs an update.

case ended

The Live Activity is visible, but a person, app, or system ended it, and it won’t update its content anymore.

### Operators

static func == (ActivityState, ActivityState) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Observing the Live Activity life cycle

var activityState: ActivityState

The current state of a Live Activity in its life cycle.

var activityStateUpdates: Activity&lt;Attributes>.ActivityStateUpdates

An asynchronous sequence you use to observe activity state changes.

struct ActivityStateUpdates

A structure that offers functionality to observe state changes of a Live Activity.

