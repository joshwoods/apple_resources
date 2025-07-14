

- PDFKit
-  PDFDisplayBox 

Enumeration

# PDFDisplayBox

The following box types may be used with `PDFPage` drawing and bounds-setting methods. See the Adobe PDF Specification for more information on box types, units, and coordinate systems.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
enum PDFDisplayBox
```

## Topics

### Constants

case mediaBox

A rectangle defining the boundaries of the physical medium for display or printing, expressed in default user-space units.

case cropBox

A rectangle defining the boundaries of the visible region , expressed in default user-space units. Default value equal to `kPDFDisplayBoxMediaBox`.

case bleedBox

A rectangle defining the boundaries of the clip region for the page contents in a production environment. Default value equal to `kPDFDisplayBoxCropBox`.

case trimBox

A rectangle defining the intended boundaries of the finished page. Default value equal to `kPDFDisplayBoxCropBox`.

case artBox

A rectangle defining the boundaries of the page’s meaningful content including surrounding white space intended for display. Default value equal to `kPDFDisplayBoxCropBox`.

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

### Supporting Types

enum PDFDisplayDirection

