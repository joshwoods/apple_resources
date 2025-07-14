

- TabularData
- RowGroupingProtocol
-  summary() 

Instance Method

# summary()

Generates a group summaries instance of the row grouping’s columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> any GroupSummaries
```

**Required**

## See Also

### Summarizing a Row Grouping

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance of the row grouping’s columns you select by name.

**Required** Default implementation provided.

protocol GroupSummaries

A collection of group summaries.

