

- TabularData
- DataFrame
- DataFrame.Slice
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns a column you select by its column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
subscript(columnID: ColumnID) -> DiscontiguousColumnSlice { get }
```

## See Also

### Creating a Slice by Selecting a Column

subscript&lt;T>(column _: Int, T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its index.

subscript&lt;T>(String, T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its name and type.

subscript(String) -> AnyColumnSlice

Returns a column you select by its name.

subscript(dynamicMember _: String) -> AnyColumnSlice

Returns a column you select by its name to support dynamic-member lookup.

