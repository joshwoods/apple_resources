

- Create ML Components
- TabularPipelineDataError
-  errorDescription 

Instance Property

# errorDescription

A localized message describing what error occurred.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
var errorDescription: String? { get }
```

## See Also

### Getting the cases

case incorrectType(operation: String, columnName: String, actual: String, expected: String)

A column has an incorrect type.

case missingColumn(operation: String, columnName: String)

A column is missing from the data frame.

case missingValues(operation: String, columnName: String)

The selected column has missing values.

