

- PDFKit
- PDFAnnotation
-  userName 

Instance Property

# userName

Returns the name of the user who created the annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var userName: String? { get set }
```

## Return Value

The name of the user who created the annotation, or NULL if no user name is set.

## See Also

### Related Documentation

class PDFAnnotation

An annotation in a PDF document.

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var modificationDate: Date?

Returns the modification date of the annotation.

var type: String?

Returns the type of the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

class PDFDestination

A `PDFDestination` object describes a point on a PDF page.

