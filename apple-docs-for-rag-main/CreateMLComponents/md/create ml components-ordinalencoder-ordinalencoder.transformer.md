

- Create ML Components
- OrdinalEncoder
-  OrdinalEncoder.Transformer 

Structure

# OrdinalEncoder.Transformer

A transformer that encodes a category as an integer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Transformer
```

Available when `Category` conforms to `Comparable`, `Decodable`, `Encodable`, and `Hashable`.

## Topics

### Creating a transformer

init(categories: Set&lt;Category?>)

Creates an ordinal encoder.

### Getting the categories

var categories: Set&lt;Category?>

Unique values to encode

func category(at: Int) -> Category?

Retrieves the category at the ordinal encoding index.

### Applying the transformation

func applied&lt;S>(S, eventHandler: EventHandler?) throws -> [Int]

Performs an ordinal encoding on a sequence of inputs.

func applied(to: Category?, eventHandler: EventHandler?) throws -> Int

Performs an ordinal encoding on a single input.

### Type Aliases

typealias Input

The input type.

typealias Output

The output type.

### Default Implementations

CustomDebugStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Transformer Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Decodable
- Encodable
- Sendable
- Transformer

