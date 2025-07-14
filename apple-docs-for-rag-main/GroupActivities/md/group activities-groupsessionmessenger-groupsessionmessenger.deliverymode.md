

- Group Activities
- GroupSessionMessenger
-  GroupSessionMessenger.DeliveryMode 

Enumeration

# GroupSessionMessenger.DeliveryMode

The transmission characteristics to apply to the delivery of messages.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
enum DeliveryMode
```

## Topics

### Getting the delivery mode options

case reliable

An attempt to ensure the delivery of messages to known participants.

case unreliable

A best-effort attempt to deliver the message to known participants.

### Comparing the delivery mode options

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == (GroupSessionMessenger.DeliveryMode, GroupSessionMessenger.DeliveryMode) -> Bool

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
- Sendable

