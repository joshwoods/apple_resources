

- Create ML Components
- TransformerToUpdatableEstimatorAdaptor
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Does nothing since this estimator uses a pre-defined transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout Transformer,
    with input: InputSequence,
    eventHandler: EventHandler? = nil
) async throws where InputSequence : Sequence, Transformer.Input == InputSequence.Element
```

## See Also

### Fitting and updating

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

func makeTransformer() -> Transformer

Creates a default-initialized transformer suitable for incremental fitting.

