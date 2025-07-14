

- Create ML Components
- ColumnSelector
-  init(columns:estimator:) 

Initializer

# init(columns:estimator:)

Creates a select operation with an estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    columns: [String],
    estimator: Estimator
)
```

## Parameters 

`columns`  

An array of columns.

`estimator`  

An estimator.

## See Also

### Creating the selection

init(ColumnSelection, estimator: Estimator)

Creates a select operation with an estimator.

init&lt;T>(ColumnSelection, transformer: T)

Creates a select operation with a transformer.

