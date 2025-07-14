

- Accelerate
- BNNS
-  BNNS.Norm Deprecated

Structure

# BNNS.Norm

Constants that describe norm types.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
@frozen
struct Norm
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Norm Types

static var taxicab: BNNS.Norm

A constant that represents the taxicab norm.

static var l1: BNNS.Norm

A constant that represents the L1 norm.

static var euclidean: BNNS.Norm

A constant that represents the Euclidean norm.

static var l2: BNNS.Norm

A constant that represents the L2 norm.

static var maximum: BNNS.Norm

A constant that represents the maximum norm.

static var lInfinity: BNNS.Norm

A constant that represents the maximum norm.

### Raw Values

init(rawValue: Float)

Creates a new instance with the specified raw value.

var rawValue: Float

The corresponding value of the raw type.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

## See Also

### Creating an Embedding Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, dictionary: BNNSNDArrayDescriptor, paddingIndex: Int, maximumNorm: Float, normType: BNNS.Norm, scalesGradientByFrequency: Bool, filterParameters: BNNSFilterParameters?)

Returns a new embedding layer.

Deprecated

