

- TabularData
- DataFrame
-  grouped(by:) 

Instance Method

# grouped(by:)

Creates a grouping from multiple columns you select by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(by columnNames: String...) -> some RowGroupingProtocol
```

## Parameters 

`columnNames`  

A comma-separated, or variadic, list of column names.

