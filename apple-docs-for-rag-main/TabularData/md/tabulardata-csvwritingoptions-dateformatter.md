

- TabularData
- CSVWritingOptions
-  dateFormatter 

Instance Property

# dateFormatter

A closure that maps dates to their string representations.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+watchOS 8.5+

``` source
var dateFormatter: (Date) -> String { get set }
```

## Discussion

Defaults to ISO 8601 encoding.

