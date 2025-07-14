

- TabularData
- DataFrame
-  grouped(by:) 

Instance Method

# grouped(by:)

Creates a grouping from multiple columns that you select by column identifier.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func grouped(by columnIDs: ColumnID...) -> some RowGroupingProtocol where T : Hashable
```

## Parameters 

`columnIDs`  

A comma-separated, or variadic, list of column identifiers.

