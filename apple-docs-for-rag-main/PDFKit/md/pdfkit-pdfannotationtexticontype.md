

- PDFKit
-  PDFAnnotationTextIconType 

Structure

# PDFAnnotationTextIconType

Constants for icon type values in text annotation property dictionaries.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationTextIconType
```

## Topics

### Choosing a Text Icon Type

static let comment: PDFAnnotationTextIconType

An icon that represents a comment.

static let key: PDFAnnotationTextIconType

An icon that represents a key.

static let note: PDFAnnotationTextIconType

An icon that represents a note.

static let help: PDFAnnotationTextIconType

An icon that indicates help information is available.

static let newParagraph: PDFAnnotationTextIconType

An icon that represents a new paragraph.

static let paragraph: PDFAnnotationTextIconType

An icon that represents a paragraph.

static let insert: PDFAnnotationTextIconType

An icon that represents an insertion command.

### Creating a Text Icon Type

init(rawValue: String)

Creates a text icon type using the specified raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Text Annotations

var iconType: PDFTextAnnotationIconType

The type of icon to display for a pop-up text annotation.

enum PDFTextAnnotationIconType

The types of icons that a text annotation can use.

