

- TabularData
- DataFrame
- DataFrame.Slice
-  summary(ofColumns:) 

Instance Method

# summary(ofColumns:)

Generates a data frame that summarizes the columns you select by index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary(ofColumns columnIndices: Int...) -> DataFrame
```

## Parameters 

`columnIndices`  

A comma-separated, or variadic, list of column indices in the data frame slice.

## See Also

### Summarizing a Slice

func summary() -> DataFrame

Generates a data frame that summarizes the columns of the data frame slice.

func summary(of: String...) -> DataFrame

Generates a data frame that summarizes the columns you select by name.

enum SummaryColumnIDs

The summary data frame column identifiers.

