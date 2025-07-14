

- TabularData
- Column
-  init(\_:) 

Initializer

# init(\_:)

Creates a column from a column slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(_ slice: ColumnSlice)
```

## Parameters 

`slice`  

A column slice.

## See Also

### Creating a Column

init(name: String, capacity: Int)

Creates a column with a name and a capacity.

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

