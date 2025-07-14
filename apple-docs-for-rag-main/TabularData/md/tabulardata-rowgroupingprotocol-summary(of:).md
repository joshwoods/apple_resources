

- TabularData
- RowGroupingProtocol
-  summary(of:) 

Instance Method

# summary(of:)

Generates a group summaries instance of the row grouping’s columns you select by name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary(of columnNames: [String]) -> any GroupSummaries
```

**Required** Default implementation provided.

## Parameters 

`columnNames`  

An array of column names.

## Default Implementations

### RowGroupingProtocol Implementations

func summary(of: String...) -> any GroupSummaries

Generates a categorical summary of the columns you select by name.

## See Also

### Summarizing a Row Grouping

func summary() -> any GroupSummaries

Generates a group summaries instance of the row grouping’s columns.

**Required**

protocol GroupSummaries

A collection of group summaries.

