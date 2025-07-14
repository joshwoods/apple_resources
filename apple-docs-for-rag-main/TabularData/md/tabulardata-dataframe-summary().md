

- TabularData
- DataFrame
-  summary() 

Instance Method

# summary()

Generates a data frame that summarizes the columns of the data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func summary() -> DataFrame
```

## See Also

### Summarizing a Data Frame

func summary(of: String...) -> DataFrame

Generates a data frame that summarizes the columns you select by name.

func summary(ofColumns: Int...) -> DataFrame

Generates a data frame that summarizes the columns you select by index.

enum SummaryColumnIDs

The summary data frame column identifiers.

