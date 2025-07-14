

- PDFKit
-  PDFAnnotationLineEndingStyle 

Structure

# PDFAnnotationLineEndingStyle

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationLineEndingStyle
```

## Topics

### Choosing a Line-Ending Style

static let circle: PDFAnnotationLineEndingStyle

A style that displays a circle line ending and fills it with the annotation’s interior color.

static let closedArrow: PDFAnnotationLineEndingStyle

A style that displays a closed arrowhead line ending and fills it with the annotation’s interior color.

static let diamond: PDFAnnotationLineEndingStyle

static let none: PDFAnnotationLineEndingStyle

static let openArrow: PDFAnnotationLineEndingStyle

A style that displays an open arrowhead line ending.

static let square: PDFAnnotationLineEndingStyle

A style that displays a square line ending and fills it with the annotation’s interior color.

### Creating a Line-Ending Style

init(rawValue: String)

Creates a line-ending style using the specified raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Line Properties

static let lineEndingStyles: PDFAnnotationKey

An array of string values that specifies the styles to use for the ends of lines.

enum PDFLineStyle

The following constants specify the available line ending styles.

static let linePoints: PDFAnnotationKey

An array of floating point values that specifies the starting and ending points, in page-space coordinates, of a line.

