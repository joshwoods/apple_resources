

- TabularData
- RowGrouping
-  summary(of:) 

Instance Method

# summary(of:)

Generates a group summaries instance for the columns you select by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary(of columnNames: [String]) -> any GroupSummaries
```

Available when `GroupingKey` conforms to `Hashable`.

## Parameters 

`columnNames`  

An array of column names.

## See Also

### Summarizing a Row Grouping

func summary() -> any GroupSummaries

Generates a group summaries instance for the columns of the row grouping.

protocol GroupSummaries

A collection of group summaries.

