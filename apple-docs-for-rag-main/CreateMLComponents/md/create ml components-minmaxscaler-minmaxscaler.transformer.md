

- Create ML Components
- MinMaxScaler
-  MinMaxScaler.Transformer 

Structure

# MinMaxScaler.Transformer

A transformer that scales the input values so that they all lie in a closed range.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Transformer
```

Available when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## Topics

### Creating a transformer

init(desiredRange: ClosedRange&lt;Element>, fittedRange: ClosedRange&lt;Element>)

Creates a minmax scaling transformer.

### Getting the properties

var desiredRange: ClosedRange&lt;Element>

The desired range of transformed values.

var fittedRange: ClosedRange&lt;Element>

The fitted range derived by the estimator when fitting.

### Performing the transformation

func applied(to: Element, eventHandler: EventHandler?) -> Element

Scales the input values so that they all lie in the closed range `[minimum, maximum]`.

### Operators

static func == (MinMaxScaler&lt;Element>.Transformer, MinMaxScaler&lt;Element>.Transformer) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable
- Transformer

