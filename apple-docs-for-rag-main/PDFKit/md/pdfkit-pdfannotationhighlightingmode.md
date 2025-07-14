

- PDFKit
-  PDFAnnotationHighlightingMode 

Structure

# PDFAnnotationHighlightingMode

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationHighlightingMode
```

## Topics

### Choosing a Highlight Mode

static let invert: PDFAnnotationHighlightingMode

A highlight mode that inverts the content of the annotation.

static let none: PDFAnnotationHighlightingMode

A highlight mode that doesn’t change the appearance of the annotation.

static let outline: PDFAnnotationHighlightingMode

A highlight mode that inverts the annotation’s border.

static let push: PDFAnnotationHighlightingMode

A highlight mode that renders a pressed appearance for the annotation.

### Creating an Annotation Highlight Mode

init(rawValue: String)

Creates a highlight mode using the specified raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Annotation Appearance

static let appearanceDictionary: PDFAnnotationKey

A dictionary that contains properties for controlling the annotation’s visual appearance.

static let appearanceState: PDFAnnotationKey

A string that specifies the appearance stream for the annotation.

static let border: PDFAnnotationKey

An array of integers or border objects that describes the border of the annotation.

static let borderStyle: PDFAnnotationKey

A dictionary that contains the properties of the annotation’s border.

static let color: PDFAnnotationKey

An array of floats or a color object that specifies the annotation’s color.

static let defaultAppearance: PDFAnnotationKey

A string value a free text annotation uses to format the text.

static let highlightingMode: PDFAnnotationKey

A string value that defines the way an annotation highlights when the user activates it, such as when clicking or tapping a link.

static let iconName: PDFAnnotationKey

A string value that specifies the name of an icon for a text or stamp annotation.

static let interiorColor: PDFAnnotationKey

An array of floating point values or a PDF color object that annotations use to fill interior space, such as line endings, squares, or circles.

static let quadding: PDFAnnotationKey

An integer value that specifies left, right, or center justification.

