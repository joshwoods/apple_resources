

- Create ML Components
- ColumnSelector
-  init(\_:estimator:) 

Initializer

# init(\_:estimator:)

Creates a select operation with an estimator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
init(
    _ columnSelection: ColumnSelection,
    estimator: Estimator
)
```

## Parameters 

`columnSelection`  

A selection of columns.

`estimator`  

An estimator.

## See Also

### Creating the selection

init(columns: [String], estimator: Estimator)

Creates a select operation with an estimator.

init&lt;T>(ColumnSelection, transformer: T)

Creates a select operation with a transformer.

