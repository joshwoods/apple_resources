

- TabularData
- CSVReadingOptions
-  nilEncodings 

Instance Property

# nilEncodings

The set of strings that stores acceptable spellings for empty values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var nilEncodings: Set
```

## Discussion

Defaults to `["", "#N/A", "#N/A N/A", "#NA", "N/A", "NA", "NULL", "n/a", "null"]`.

