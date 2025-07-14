

- TabularData
- AnyColumn
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Appends the contents of another column to the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func append(contentsOf other: AnyColumn)
```

## Parameters 

`other`  

A column that contains elements of the same type as this column.

## See Also

### Adding Elements

func append(Any?)

Appends an optional element to the column.

func append(contentsOf: AnyColumnSlice)

Appends the contents of a column slice to the column.

