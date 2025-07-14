

- TabularData
- DataFrameProtocol
-  description(options:) 

Instance Method

# description(options:)

Generates a text representation of the data frame type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func description(options: FormattingOptions) -> String
```

## Parameters 

`options`  

A set of formatting options that affect the description string, including the maximum width of a column and the maximum number of rows.

## Discussion

`FormattingOptions.maximumLineWidth` needs to be wide enough to print at least the index column, the truncation column, and one data column (at least two characters, one for initial of the content, and one for “…”).

