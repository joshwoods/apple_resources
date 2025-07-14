

- PDFKit
- PDFAnnotationKey
-  parent 

Type Property

# parent

A dictionary or annotation object that a pop-up or widget belongs to.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
static let parent: PDFAnnotationKey
```

## See Also

### Configuring General Properties

static let contents: PDFAnnotationKey

The text that the annotation displays or represents.

static let date: PDFAnnotationKey

The date, or string representation of a date, of the annotation’s most recent modification.

static let flags: PDFAnnotationKey

An integer value that specifies flags for the annotation.

static let name: PDFAnnotationKey

A string that uniquely identifies the annotation among all annotations on the same page.

static let page: PDFAnnotationKey

A dictionary or PDF page object that includes the annotation.

static let quadPoints: PDFAnnotationKey

An array of floating point values that specifies a rectangular region of a page.

static let rect: PDFAnnotationKey

The rectangle that the annotation occupies on the page, in page-space coordinates.

static let subtype: PDFAnnotationKey

The type of annotation that the entries in a dictionary describe.

static let textLabel: PDFAnnotationKey

A string that represents the title of the annotation.

