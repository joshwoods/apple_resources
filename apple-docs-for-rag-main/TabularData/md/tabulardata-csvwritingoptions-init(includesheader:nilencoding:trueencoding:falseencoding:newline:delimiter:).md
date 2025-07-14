

- TabularData
- CSVWritingOptions
-  init(includesHeader:nilEncoding:trueEncoding:falseEncoding:newline:delimiter:) 

Initializer

# init(includesHeader:nilEncoding:trueEncoding:falseEncoding:newline:delimiter:)

Creates a set of options for writing a CSV file.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    includesHeader: Bool = true,
    nilEncoding: String = "",
    trueEncoding: String = "true",
    falseEncoding: String = "false",
    newline: String = "\n",
    delimiter: Character = ","
)
```

## Parameters 

`includesHeader`  

A Boolean value that indicates whether to write a header with the column names. Defaults to `true`.

`nilEncoding`  

The spelling for nil values. Defaults to an empty string.

`trueEncoding`  

The spelling for true Boolean values. Defaults to `true`.

`falseEncoding`  

The spelling for false Boolean values. Defaults to `false`.

`newline`  

The newline sequence. Defaults to a line feed.

`delimiter`  

The field delimiter. Defaults to comma (`,`).

