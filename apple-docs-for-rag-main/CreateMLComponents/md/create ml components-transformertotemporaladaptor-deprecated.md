

- Create ML Components
-  TransformerToTemporalAdaptor Deprecated

Structure

# TransformerToTemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
struct TransformerToTemporalAdaptor where Base : Transformer
```

## Topics

### Creating a transformer

init(Base)

Creates a temporal transformer from a transformer.

### Applying

func applied&lt;S>(to: S, eventHandler: EventHandler?) async throws -> AnyTemporalSequence&lt;TransformerToTemporalAdaptor&lt;Base>.Output>

Performs the transformation on each element of the input sequence.

typealias Input

The input type.

typealias Output

The output type.

typealias OutputSequence

The output sequence type.

### Default Implementations

TemporalTransformer Implementations

## Relationships

### Conforms To

- Sendable
- TemporalTransformer

## See Also

### Transformer adaptors

struct TransformerToEstimatorAdaptor

An estimator that always returns a predefined transformer.

struct TransformerToUpdatableEstimatorAdaptor

An updatable estimator that always returns a predefined transformer.

