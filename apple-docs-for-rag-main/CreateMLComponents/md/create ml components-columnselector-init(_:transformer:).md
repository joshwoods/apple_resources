

- Create ML Components
- ColumnSelector
-  init(\_:transformer:) 

Initializer

# init(\_:transformer:)

Creates a select operation with a transformer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    _ columnSelection: ColumnSelection,
    transformer: T
) where Estimator == TransformerToEstimatorAdaptor, T : Transformer, T.Input == UnwrappedInput?
```

## Parameters 

`columnSelection`  

A selection of columns.

`transformer`  

A transformer.

## See Also

### Creating the selection

init(columns: [String], estimator: Estimator)

Creates a select operation with an estimator.

init(ColumnSelection, estimator: Estimator)

Creates a select operation with an estimator.

