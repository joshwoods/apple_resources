

- TabularData
- RowGrouping
-  summary() 

Instance Method

# summary()

Generates a group summaries instance for the columns of the row grouping.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> any GroupSummaries
```

Available when `GroupingKey` conforms to `Hashable`.

## See Also

### Summarizing a Row Grouping

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance for the columns you select by name.

protocol GroupSummaries

A collection of group summaries.

