

- TabularData
- DataFrame
- DataFrame.Slice
-  subscript(column:\_:) 

Instance Subscript

# subscript(column:\_:)

Returns a column you select by its index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(column index: Int, type: T.Type) -> DiscontiguousColumnSlice { get }
```

## Parameters 

`index`  

The index of a column.

## See Also

### Creating a Slice by Selecting a Column

subscript&lt;T>(ColumnID&lt;T>) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its column identifier.

subscript&lt;T>(String, T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its name and type.

subscript(String) -> AnyColumnSlice

Returns a column you select by its name.

subscript(dynamicMember _: String) -> AnyColumnSlice

Returns a column you select by its name to support dynamic-member lookup.

