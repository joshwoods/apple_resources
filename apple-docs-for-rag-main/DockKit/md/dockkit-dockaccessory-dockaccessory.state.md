

- DockKit
- DockAccessory
-  DockAccessory.State 

Enumeration

# DockAccessory.State

The state of a dock accessory.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum State
```

## Topics

### Getting properties

case docked

The dock accessory doesn’t contain a device.

case undocked

The dock accessory contains a device.

var debugDescription: String

The text description of the dock accessory state.

### Operators

static func == (DockAccessory.State, DockAccessory.State) -> Bool

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

- CustomDebugStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Getting accessory information

var firmwareVersion: String?

The firmware version of the dock accessory.

var hardwareModel: String?

The model of the dock accessory.

let identifier: DockAccessory.Identifier

The name and unique identifer of the dock accessory.

struct Identifier

Information that uniquely identifies the dock accessory.

enum Category

Types of supported dock accesories.

struct StateChange

An event that indicates a change in the state of a dock accessory.

struct StateChanges

An asynchronous sequence of dock accessory state changes.

