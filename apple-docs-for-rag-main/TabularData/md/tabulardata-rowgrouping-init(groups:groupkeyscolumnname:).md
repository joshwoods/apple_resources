

- TabularData
- RowGrouping
-  init(groups:groupKeysColumnName:) 

Initializer

# init(groups:groupKeysColumnName:)

Creates a row grouping from a list of groups.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    groups: [(GroupingKey?, D)],
    groupKeysColumnName: String
) where D : DataFrameProtocol
```

## Parameters 

`groups`  

An array of tuples. Each tuple pairs a key with a data frame type.

`groupKeysColumnName`  

The name of the grouping key column the row grouping creates when it generates a data frame, such as its ungrouped() or counts(order:) methods.

## Discussion

The member data frames must all have the same columns (count, names, and types).

## See Also

### Creating a Row Grouping

init&lt;D>(frame: D, columnName: String, timeUnit: Calendar.Component)

Creates a row grouping from a column with date or time elements.

