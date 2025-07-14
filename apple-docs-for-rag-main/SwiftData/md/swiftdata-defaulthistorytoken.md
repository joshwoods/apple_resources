

- SwiftData
-  DefaultHistoryToken 

Structure

# DefaultHistoryToken

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+Swift 5.9+

``` source
struct DefaultHistoryToken
```

## Topics

### Operators

static func == (DefaultHistoryToken, DefaultHistoryToken) -> Bool

Returns a Boolean value indicating whether two values are equal.

static func &lt; (DefaultHistoryToken, DefaultHistoryToken) -> Bool

Returns a Boolean value indicating whether the value of the first argument is less than that of the second argument.

### Initializers

init(from: any Decoder) throws

Creates a new instance by decoding from the given decoder.

### Instance Properties

var hashValue: Int

The hash value.

var id: Int

The stable identity of the entity associated with this instance.

var tokenValue: DefaultHistoryToken.TokenType?

### Instance Methods

func encode(to: any Encoder) throws

Encodes this value into the given encoder.

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

typealias TokenType

### Default Implementations

Comparable Implementations

Equatable Implementations

## Relationships

### Conforms To

- Comparable
- Decodable
- Encodable
- Equatable
- Hashable
- HistoryToken
- Identifiable
- Sendable

