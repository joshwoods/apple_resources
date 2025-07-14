

- Create ML Components
- TransformerToUpdatableEstimatorAdaptor
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> Transformer
```

## See Also

### Fitting and updating

func fitted&lt;S>(to: S, eventHandler: EventHandler?) async throws -> Transformer

Returns the pre-defined transformer.

func update&lt;InputSequence>(inout Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Does nothing since this estimator uses a pre-defined transformer.

