

- TabularData
- DataFrame
-  init(columns:) 

Initializer

# init(columns:)

Creates a new data frame from a sequence of columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(columns: S) where S : Sequence, S.Element == AnyColumn
```

## Parameters 

`columns`  

A sequence of type-erased columns.

## See Also

### Creating a Data Frame

init()

Creates an empty data frame with no rows or columns.

init(dictionaryLiteral: (String, [Any?])...)

Creates a data frame from a dictionary literal.

