

- TabularData
- CSVReadingOptions
-  usesQuoting 

Instance Property

# usesQuoting

A Boolean value that indicates whether to enable quoting.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var usesQuoting: Bool
```

## Discussion

When `true`, the contents of a quoted field can contain special characters, such as the field delimiter and newlines. Defaults to `true`.

