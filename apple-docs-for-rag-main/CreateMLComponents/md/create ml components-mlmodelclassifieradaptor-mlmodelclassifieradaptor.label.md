

- Create ML Components
- MLModelClassifierAdaptor
-  MLModelClassifierAdaptor.Label 

Enumeration

# MLModelClassifierAdaptor.Label

The classifier label type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum Label
```

## Topics

### Label types

case int(Int)

The label is integer type.

case string(String)

The label is string type.

### Operators

static func == (MLModelClassifierAdaptor&lt;Scalar>.Label, MLModelClassifierAdaptor&lt;Scalar>.Label) -> Bool

Returns a Boolean value indicating whether two values are equal.

### Instance Properties

var hashValue: Int

The hash value.

### Instance Methods

func hash(into: inout Hasher)

Hashes the essential components of this value by feeding them into the given hasher.

### Default Implementations

CustomDebugStringConvertible Implementations

Equatable Implementations

ExpressibleByExtendedGraphemeClusterLiteral Implementations

ExpressibleByIntegerLiteral Implementations

ExpressibleByStringLiteral Implementations

ExpressibleByUnicodeScalarLiteral Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Equatable
- ExpressibleByExtendedGraphemeClusterLiteral
- ExpressibleByIntegerLiteral
- ExpressibleByStringLiteral
- ExpressibleByUnicodeScalarLiteral
- Hashable
- Sendable

## See Also

### Performing the transformation

func applied(to: MLShapedArray&lt;Scalar>, eventHandler: EventHandler?) async throws -> ClassificationDistribution&lt;MLModelClassifierAdaptor&lt;Scalar>.Label>

Performs a prediction from a single input.

