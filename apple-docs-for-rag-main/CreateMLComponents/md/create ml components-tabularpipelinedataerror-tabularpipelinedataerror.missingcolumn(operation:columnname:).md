

- Create ML Components
- TabularPipelineDataError
-  TabularPipelineDataError.missingColumn(operation:columnName:) 

Case

# TabularPipelineDataError.missingColumn(operation:columnName:)

A column is missing from the data frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
case missingColumn(
    operation: String,
    columnName: String
)
```

## See Also

### Getting the cases

case incorrectType(operation: String, columnName: String, actual: String, expected: String)

A column has an incorrect type.

case missingValues(operation: String, columnName: String)

The selected column has missing values.

var errorDescription: String?

A localized message describing what error occurred.

