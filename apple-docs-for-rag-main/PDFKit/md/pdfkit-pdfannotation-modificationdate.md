

- PDFKit
- PDFAnnotation
-  modificationDate 

Instance Property

# modificationDate

Returns the modification date of the annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var modificationDate: Date? { get set }
```

## Return Value

The modification date of the annotation, or `NULL` if there is no modification date.

## See Also

### Related Documentation

class PDFAnnotation

An annotation in a PDF document.

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var userName: String?

Returns the name of the user who created the annotation.

var type: String?

Returns the type of the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

class PDFDestination

A `PDFDestination` object describes a point on a PDF page.

