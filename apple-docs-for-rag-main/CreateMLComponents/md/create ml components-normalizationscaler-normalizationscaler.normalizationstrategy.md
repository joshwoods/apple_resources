

- Create ML Components
- NormalizationScaler
-  NormalizationScaler.NormalizationStrategy 

Enumeration

# NormalizationScaler.NormalizationStrategy

A normalization strategy.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
enum NormalizationStrategy
```

## Topics

### Normalization strategies

case l1

A normalization strategy that scales by the L1 Norm (sum of vector absolute values).

case l2

A normalization strategy that scales by the L2 Norm (Euclidean norm).

### Operators

static func == (NormalizationScaler&lt;Element>.NormalizationStrategy, NormalizationScaler&lt;Element>.NormalizationStrategy) -> Bool

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

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a scaler

init(norm: NormalizationScaler&lt;Element>.NormalizationStrategy)

Creates a normalization scaler.

