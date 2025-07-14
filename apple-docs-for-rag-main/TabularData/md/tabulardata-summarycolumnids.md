

- TabularData
-  SummaryColumnIDs 

Enumeration

# SummaryColumnIDs

The summary data frame column identifiers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum SummaryColumnIDs
```

## Topics

### Type Properties

static let columnName: ColumnID&lt;String>

The identifier that represents the summary’s column that contains the column names in a data frame.

static let firstQuartile: ColumnID&lt;Double>

The identifier that represents the summary’s column of first quartiles.

static let maximum: ColumnID&lt;Double>

The identifier that represents the summary’s column of maximums.

static let mean: ColumnID&lt;Double>

The identifier that represents the summary’s column of arithmetic means.

static let median: ColumnID&lt;Double>

The identifier that represents the summary’s column of medians.

static let minimum: ColumnID&lt;Double>

The identifier that represents the summary’s column of minimums.

static let mode: ColumnID&lt;[Any]>

The identifier that represents the summary’s column of most frequent elements.

static let noneCount: ColumnID&lt;Int>

The identifier that represents the summary’s column of missing counts.

static let someCount: ColumnID&lt;Int>

The identifier that represents the summary’s column of non-missing counts.

static let standardDeviation: ColumnID&lt;Double>

The identifier that represents the summary’s column of standard deviations.

static let thirdQuartile: ColumnID&lt;Double>

The identifier that represents the summary’s column of third quartiles.

static let uniqueCount: ColumnID&lt;Int>

The identifier that represents the summary’s column of unique counts.

## Relationships

### Conforms To

- Sendable

## See Also

### Summarizing a Data Frame

func summary() -> DataFrame

Generates a data frame that summarizes the columns of the data frame.

func summary(of: String...) -> DataFrame

Generates a data frame that summarizes the columns you select by name.

func summary(ofColumns: Int...) -> DataFrame

Generates a data frame that summarizes the columns you select by index.

