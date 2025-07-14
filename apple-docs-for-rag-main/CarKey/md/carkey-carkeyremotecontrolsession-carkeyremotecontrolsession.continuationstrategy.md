

- CarKey
- CarKeyRemoteControlSession
-  CarKeyRemoteControlSession.ContinuationStrategy 

Enumeration

# CarKeyRemoteControlSession.ContinuationStrategy

Strategy to use on reception of a continuation request.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+watchOS 11.0+

``` source
enum ContinuationStrategy
```

## Topics

### Operators

static func == (CarKeyRemoteControlSession.ContinuationStrategy, CarKeyRemoteControlSession.ContinuationStrategy) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Enumeration Cases

case automatic

Auto-confirm any incoming continuation requests until the requested action is stopped or completed with no intervention from the client.

case manual

Give your app control over the incoming continuation requests and allow to exchange data with the vehicle.

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

