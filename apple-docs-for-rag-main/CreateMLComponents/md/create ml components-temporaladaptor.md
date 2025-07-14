

- Create ML Components
-  TemporalAdaptor 

Structure

# TemporalAdaptor

A temporal transformer that applies a regular transformer to each value of a temporal sequence.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct TemporalAdaptor where Base : Transformer, Base : Sendable
```

## Topics

### Initializers

init(Base)

Creates a temporal transformer from a transformer.

### Instance Methods

func applied(to: some TemporalSequence&lt;Base.Input>, eventHandler: EventHandler?) async throws -> AnyTemporalSequence&lt;TemporalAdaptor&lt;Base>.Output>

Performs the transformation on each element of the input sequence.

### Type Aliases

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

### Temporal adaptors

struct TemporalTransformerToEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

struct TemporalEstimatorToSupervisedAdaptor

An adaptor that exposes a temporal estimator as a supervised temporal estimator.

Deprecated

struct TemporalTransformerToUpdatableEstimatorAdaptor

A temporal estimator that always returns a predefined temporal transformer.

Deprecated

