

- Create ML Components
- UpdatableEstimatorToTemporalAdaptor
-  UpdatableEstimatorToTemporalAdaptor.Input Deprecated

Type Alias

# UpdatableEstimatorToTemporalAdaptor.Input

The input type.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
typealias Input = Base.Transformer.Input
```

## See Also

### Fitting and updating

func fitted&lt;InputSequence>(to: InputSequence, eventHandler: EventHandler?) async throws -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Fits a transformer to a sequence of examples.

Deprecated

func makeTransformer() -> UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

Deprecated

func update&lt;InputSequence>(inout UpdatableEstimatorToTemporalAdaptor&lt;Base>.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

Deprecated

typealias Output

The output type.

Deprecated

typealias Transformer

The transformer type created by this estimator.

Deprecated

