

- Create ML Components
- UpdatableTabularEstimator
-  makeTransformer() 

Instance Method

# makeTransformer()

Creates a default-initialized transformer suitable for incremental fitting.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func makeTransformer() -> Self.Transformer
```

**Required**

## See Also

### Transforming

func update(inout Self.Transformer, with: DataFrame) async throws

func update(inout Self.Transformer, with: DataFrame, eventHandler: EventHandler?) async throws

Updates a transformer with a new sequence of examples.

**Required**

