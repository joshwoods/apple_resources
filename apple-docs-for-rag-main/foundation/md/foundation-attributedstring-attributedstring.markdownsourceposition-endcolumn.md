

- Foundation
- AttributedString
- AttributedString.MarkdownSourcePosition
-  endColumn 

Instance Property

# endColumn

The column where the text ends in the Markdown source.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
let endColumn: Int
```

## Discussion

This property uses `1`-based counting. Columns represent UTF-8 indices; for multi-byte characters, the column indicates the first byte.

## See Also

### Inspecting Markdown Source Position Properties

let startLine: Int

The line where the text begins in the Markdown source.

let startColumn: Int

The column where the text begins in the Markdown source.

let endLine: Int

The line where the text ends in the Markdown source.

