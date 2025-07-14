

- TabularData
- Column
-  init(name:contents:) 

Initializer

# init(name:contents:)

Creates a column with a name and a sequence of nonoptional values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    name: String,
    contents: S
) where WrappedElement == S.Element, S : Sequence
```

## Parameters 

`name`  

A column name.

`contents`  

A sequence of nonoptional elements.

## See Also

### Creating a Column

init(name: String, capacity: Int)

Creates a column with a name and a capacity.

init(ColumnID&lt;WrappedElement>, capacity: Int)

Creates a column with a column identifier and a capacity.

init&lt;S>(name: String, contents: S)

Creates a column with a name and a sequence of optional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with an identifier and a sequence of nonoptional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with a column identifier and a sequence of optional values.

init(ColumnSlice&lt;WrappedElement>)

Creates a column from a column slice.

