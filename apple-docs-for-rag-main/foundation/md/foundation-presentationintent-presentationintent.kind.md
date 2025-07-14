

- Foundation
- PresentationIntent
-  PresentationIntent.Kind 

Enumeration

# PresentationIntent.Kind

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Kind
```

## Topics

### Enumeration Cases

case blockQuote

case codeBlock(languageHint: String?)

case header(level: Int)

case listItem(ordinal: Int)

case orderedList

case paragraph

case table(columns: [PresentationIntent.TableColumn])

case tableCell(columnIndex: Int)

case tableHeaderRow

case tableRow(rowIndex: Int)

case thematicBreak

case unorderedList

## Relationships

### Conforms To

- CustomDebugStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

