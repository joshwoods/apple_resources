

- Create ML Components
- UpdatableEstimator
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout Self.Transformer,
    with input: InputSequence,
    eventHandler: EventHandler?
) async throws where InputSequence : Sequence, InputSequence.Element == Self.Transformer.Input
```

**Required**

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

## See Also

### Transforming

func makeTransformer() -> Self.Transformer

Creates a default-initialized transformer suitable for incremental fitting.

**Required**

func update&lt;InputSequence>(inout Self.Transformer, with: InputSequence) async throws

