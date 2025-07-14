

- Create ML Components
- UpdatableSupervisedTemporalEstimator
-  makeTransformer() Deprecated

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 16.0–18.0DeprecatediPadOS 16.0–18.0DeprecatedMac Catalyst 16.0–18.0DeprecatedmacOS 13.0–15.0DeprecatedtvOS 16.0–18.0DeprecatedvisionOS 1.0–2.0Deprecated

``` source
func makeTransformer() -> Self.Transformer
```

**Required**

## See Also

### Transforming

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required**

Deprecated

func update&lt;InputSequence, FeatureSequence>(inout Self.Transformer, with: InputSequence) async throwsDeprecated

