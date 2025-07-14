

- Create ML Components
- NormalizationScaler
-  NormalizationScaler.Transformer 

Structure

# NormalizationScaler.Transformer

A transformer that scales the input using a normalization strategy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Transformer
```

Available when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## Topics

### Creating a transformer

init(scale: Element)

Creates a normalization scaling transformer.

### Getting the scale

var scale: Element

The normalization scale used to scale the input.

### Performing the transformation

func applied(to: Element, eventHandler: EventHandler?) -> Element

Scales the input values using the calculation `input / scale`.

### Operators

static func == (NormalizationScaler&lt;Element>.Transformer, NormalizationScaler&lt;Element>.Transformer) -> Bool

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

