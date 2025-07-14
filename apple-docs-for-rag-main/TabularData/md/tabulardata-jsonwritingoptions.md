

- TabularData
-  JSONWritingOptions 

Structure

# JSONWritingOptions

A set of JSON file-reading options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct JSONWritingOptions
```

## Topics

### Initializers

init()

Creates a set of options for writing a JSON file.

### Instance Properties

var dateFormatter: (Date) -> String

A closure that maps dates to their string representations.

var prettyPrint: Bool

A Boolean value that indicates whether to split lines and indent the generated JSON.

var sortKeys: Bool

A Boolean value that indicates whether to sort the keys.

