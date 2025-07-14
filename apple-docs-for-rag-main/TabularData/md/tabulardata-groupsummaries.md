

- TabularData
-  GroupSummaries 

Protocol

# GroupSummaries

A collection of group summaries.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol GroupSummaries : CustomStringConvertible
```

## Topics

### Instance Properties

var description: String

A text representation of the group summaries.

**Required**

### Instance Methods

func description(options: FormattingOptions) -> String

Generates a text representation of the group summaries.

**Required**

### Subscripts

subscript(Any?...) -> DataFrame?

Retrieves one or more summaries by their group keys.

**Required**

## Relationships

### Inherits From

- CustomStringConvertible

## See Also

### Summarizing a Row Grouping

func summary() -> any GroupSummaries

Generates a group summaries instance for the columns of the row grouping.

func summary(of: [String]) -> any GroupSummaries

Generates a group summaries instance for the columns you select by name.

