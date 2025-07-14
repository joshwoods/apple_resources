

- Create ML Components
- StandardScaler
-  StandardScaler.Transformer 

Structure

# StandardScaler.Transformer

A transformer that standardizes the input by removing the mean and scaling to unit variance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Transformer
```

Available when `Element` conforms to `BinaryFloatingPoint`, `Decodable`, and `Encodable`.

## Topics

### Creating a transformer

init(mean: Element, standardDeviation: Element)

Creates a standard scaling transformer.

### Getting the properties

var mean: Element

The mean used for offsetting.

var standardDeviation: Element

The standard deviation used for scaling.

### Performing the transformation

func applied(to: Element, eventHandler: EventHandler?) -> Element

Scales the input values using the calculation `(input - mean) / standardDeviation`.

### Operators

static func == (StandardScaler&lt;Element>.Transformer, StandardScaler&lt;Element>.Transformer) -> Bool

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

