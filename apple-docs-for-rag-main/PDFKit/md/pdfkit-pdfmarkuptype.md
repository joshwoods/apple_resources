

- PDFKit
-  PDFMarkupType 

Enumeration

# PDFMarkupType

The styles available for markup annotations in PDFKit.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
enum PDFMarkupType
```

## Topics

### Constants

case highlight

Highlight style for the markup.

case strikeOut

Strikethrough style for the markup.

case underline

Underline style for the markup.

case redact

The redaction style for markup.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Text Markup Annotations

var markupType: PDFMarkupType

The markup type that the annotation displays, either highlight, strikethrough, underline, or redact.

var quadrilateralPoints: [NSValue]?

An array of values that represents the points bounding the marked-up text.

