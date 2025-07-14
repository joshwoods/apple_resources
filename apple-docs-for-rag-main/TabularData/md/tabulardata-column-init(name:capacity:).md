

- TabularData
- Column
-  init(name:capacity:) 

Initializer

# init(name:capacity:)

Creates a column with a name and a capacity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    name: String,
    capacity: Int
)
```

## Parameters 

`name`  

A column name.

`capacity`  

An integer that represents the number of elements the column can initially store.

## See Also

### Creating a Column

init(ColumnID&lt;WrappedElement>, capacity: Int)

Creates a column with a column identifier and a capacity.

init&lt;S>(name: String, contents: S)

Creates a column with a name and a sequence of nonoptional values.

init&lt;S>(name: String, contents: S)

Creates a column with a name and a sequence of optional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with an identifier and a sequence of nonoptional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with a column identifier and a sequence of optional values.

init(ColumnSlice&lt;WrappedElement>)

Creates a column from a column slice.

