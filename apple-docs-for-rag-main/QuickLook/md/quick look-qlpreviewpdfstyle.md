

- Quick Look
-  QLPreviewPDFStyle 

Structure

# QLPreviewPDFStyle

A value you use to configure the appearance of previews for PDF files.

macOS 10.5+

``` source
struct QLPreviewPDFStyle
```

## Topics

### Creating a Preview Style for PDF Files

init(UInt32)

Creates a PDF style instance that configures the layout of previews for PDF files.

init(rawValue: UInt32)

Creates a PDF style instance that configures the layout of previews for PDF files.

var rawValue: UInt32

The raw value that represents the layout of previews for PDF files.

### Styles for PDF Previews

var kQLPreviewPDFStandardStyle: QLPreviewPDFStyle

The PDF appears in the operating system’s standard style.

var kQLPreviewPDFPagesWithThumbnailsOnLeftStyle: QLPreviewPDFStyle

The content of the PDF appears with thumbnails of all pages on the left side of the current page’s content.

var kQLPreviewPDFPagesWithThumbnailsOnRightStyle: QLPreviewPDFStyle

The content of the PDF appears with thumbnails of all pages on the right side of the current page’s content.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

