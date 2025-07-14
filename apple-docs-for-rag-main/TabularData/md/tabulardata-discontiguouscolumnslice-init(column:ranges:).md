

- TabularData
- DiscontiguousColumnSlice
-  init(column:ranges:) 

Initializer

# init(column:ranges:)

Creates a slice with the contents of a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    column: Column,
    ranges: [Range]
)
```

## Parameters 

`column`  

A column.

`ranges`  

An array of integer ranges.

## See Also

### Creating a Column Slice

init(Column&lt;WrappedElement>)

Creates a slice with the contents of a column.

