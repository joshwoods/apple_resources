

- Foundation
- AttributedString
-  AttributedString.MarkdownSourcePosition 

Structure

# AttributedString.MarkdownSourcePosition

The position of attributed string text in its original Markdown source string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MarkdownSourcePosition
```

## Topics

### Creating a Markdown Source Position

init(startLine: Int, startColumn: Int, endLine: Int, endColumn: Int)

Creates a Markdown source position instance from its start and end line and column.

### Inspecting Markdown Source Position Properties

let startLine: Int

The line where the text begins in the Markdown source.

let startColumn: Int

The column where the text begins in the Markdown source.

let endLine: Int

The line where the text ends in the Markdown source.

let endColumn: Int

The column where the text ends in the Markdown source.

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

