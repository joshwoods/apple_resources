

- Create ML Components
- ColumnSelector
-  update(\_:with:eventHandler:) 

Instance Method

# update(\_:with:eventHandler:)

Updates a transformer with a new sequence of examples.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 11.0+

``` source
func update(
    _ transformer: inout ColumnSelector.Transformer,
    with input: DataFrame,
    eventHandler: EventHandler? = nil
) async throws
```

Available when `Estimator` conforms to `UpdatableEstimator` and `Estimator.Transformer.Input` is `UnwrappedInput?`.

## Parameters 

`transformer`  

A transformer to update.

`input`  

A sequence of examples.

`eventHandler`  

An event handler.

