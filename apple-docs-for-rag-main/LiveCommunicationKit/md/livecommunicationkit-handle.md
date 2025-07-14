

- LiveCommunicationKit
-  Handle 

Structure

# Handle

Uniquely identifies a member in a `Conversation`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
struct Handle
```

## Topics

### Operators

static func == (Handle, Handle) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

init(type: Handle.Kind, value: String, displayName: String?)

Creates a new `Handle`.

### Instance Properties

var displayName: String

The value that should be displayed to the user at the UI layer.

var hashValue: Int

The hash value.

var type: Handle.Kind

The type of handle (e.g. a phone number or email address)

var value: String

The raw value of the handle.

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Enumerations

enum Kind

The type of the handle.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

