

- Core Bluetooth
-  CBConnectionEventMatchingOption 

Structure

# CBConnectionEventMatchingOption

A set of options to use when registering for connection events.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 4.0+

``` source
struct CBConnectionEventMatchingOption
```

## Topics

### Creating a Matching Option Instance

init(rawValue: String)

Creates a matching option from the provided raw value.

### Matching Options

static let peripheralUUIDs: CBConnectionEventMatchingOption

An array of UUID objects that represents peripherals to match.

static let serviceUUIDs: CBConnectionEventMatchingOption

An array that represents service identifiers to match.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Receiving Connection Events

func registerForConnectionEvents(options: [CBConnectionEventMatchingOption : Any]?)

Register for an event notification when the central manager makes a connection matching the given options.

Peripheral Connection Options

Keys used to pass options when connecting to a peripheral.

enum CBConnectionEvent

A change to the connection state of a peer.

