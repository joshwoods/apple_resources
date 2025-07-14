

- DockKit
- DockAccessory
-  DockAccessory.Category 

Enumeration

# DockAccessory.Category

Types of supported dock accesories.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
enum Category
```

## Topics

### Getting properties

case trackingStand

The dock accessory is a tracking stand.

var debugDescription: String

The text description of the dock accessory state.

### Operators

static func == (DockAccessory.Category, DockAccessory.Category) -> Bool

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

- CustomDebugStringConvertible
- Decodable
- Encodable
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

enum State

The state of a dock accessory.

struct StateChange

An event that indicates a change in the state of a dock accessory.

struct StateChanges

An asynchronous sequence of dock accessory state changes.

