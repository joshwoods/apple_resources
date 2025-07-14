

- PDFKit
-  PDFLineStyle 

Enumeration

# PDFLineStyle

The following constants specify the available line ending styles.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
enum PDFLineStyle
```

## Topics

### Constants

case none

No line ending.

case square

A square line ending filled with the annotation’s interior color, if any.

case circle

A circular line ending filled with the annotation’s interior color, if any.

case diamond

A diamond-shaped line ending filled with the annotation’s interior color, if any.

case openArrow

An open arrowhead line ending, composed from two short lines meeting in an acute angle at the line end.

case closedArrow

A closed arrowhead line ending, consisting of a triangle with the acute vertex at the line end and filled with the annotation’s interior color, if any.

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

### Configuring Line Properties

static let lineEndingStyles: PDFAnnotationKey

An array of string values that specifies the styles to use for the ends of lines.

static let linePoints: PDFAnnotationKey

An array of floating point values that specifies the starting and ending points, in page-space coordinates, of a line.

struct PDFAnnotationLineEndingStyle

