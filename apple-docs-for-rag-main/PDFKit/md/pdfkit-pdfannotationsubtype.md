

- PDFKit
-  PDFAnnotationSubtype 

Structure

# PDFAnnotationSubtype

The type of annotation, such as circle, text, or ink.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationSubtype
```

## Topics

### Choosing an Annotation Subtype

static let circle: PDFAnnotationSubtype

An annotation that renders a circle shape.

static let freeText: PDFAnnotationSubtype

An annotation that displays an editable text field.

static let highlight: PDFAnnotationSubtype

An annotation that highlights text.

static let ink: PDFAnnotationSubtype

An annotation that represents a freehand scribble.

static let line: PDFAnnotationSubtype

An annotation that displays a single straight line.

static let link: PDFAnnotationSubtype

An annotation that provides a hyperlink to a location in the document, or an action to perform when the user clicks or taps it.

static let popup: PDFAnnotationSubtype

An annotation that displays text in a pop-up window for entry and editing.

static let square: PDFAnnotationSubtype

An annotation that displays a square shape.

static let stamp: PDFAnnotationSubtype

An annotation that displays text or a graphic as if a rubber stamp imprints it on the page.

static let strikeOut: PDFAnnotationSubtype

An annotation that strikes out text.

static let text: PDFAnnotationSubtype

An annotation that displays a collapsible note that contains text.

static let underline: PDFAnnotationSubtype

An annotation that underlines text.

static let widget: PDFAnnotationSubtype

An annotation that displays interactive form elements, including text or signature fields, radio buttons, checkboxes, push buttons, pop-ups, and tables.

### Creating an Annotation Subtype

init(rawValue: String)

Creates an annotation subtype using the specified raw string.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating an Annotation

init(bounds: CGRect, forType: PDFAnnotationSubtype, withProperties: [AnyHashable : Any]?)

Creates a PDF annotation with the specified bounds, type, and optional properties.

