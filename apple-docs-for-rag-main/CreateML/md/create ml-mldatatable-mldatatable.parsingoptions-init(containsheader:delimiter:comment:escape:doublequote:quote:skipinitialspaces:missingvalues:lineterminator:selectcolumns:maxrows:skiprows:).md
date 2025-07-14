

- Create ML
- MLDataTable
- MLDataTable.ParsingOptions
-  init(containsHeader:delimiter:comment:escape:doubleQuote:quote:skipInitialSpaces:missingValues:lineTerminator:selectColumns:maxRows:skipRows:) 

Initializer

# init(containsHeader:delimiter:comment:escape:doubleQuote:quote:skipInitialSpaces:missingValues:lineTerminator:selectColumns:maxRows:skipRows:)

Creates CSV parsing options.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(
    containsHeader: Bool = true,
    delimiter: String = ",",
    comment: String = "",
    escape: String = "\\",
    doubleQuote: Bool = true,
    quote: String = "\"",
    skipInitialSpaces: Bool = true,
    missingValues: [String] = ["NA"],
    lineTerminator: String = "\n",
    selectColumns: [String]? = nil,
    maxRows: Int? = nil,
    skipRows: Int = 0
)
```

