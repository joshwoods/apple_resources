

- PDFKit
- PDFAnnotation
-  type 

Instance Property

# type

Returns the type of the annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var type: String? { get set }
```

## Return Value

The type of the annotation. Types include `Line`, `Link`, `Text`, and so on, referring to the `PDFAnnotation` subclasses. In the Adobe PDF Specification, this attribute is called `Subtype`, and the common “type” for all annotations in the PDF Specification is `Annot`.

## See Also

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var modificationDate: Date?

Returns the modification date of the annotation.

var userName: String?

Returns the name of the user who created the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

class PDFDestination

A `PDFDestination` object describes a point on a PDF page.

