

- Create ML
- MLUntypedColumn
-  materialize() 

Instance Method

# materialize()

Creates a new column by immediately evaluating any lazily applied data processing operations stored in the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func materialize() throws -> MLUntypedColumn
```

## Return Value

A new column.

