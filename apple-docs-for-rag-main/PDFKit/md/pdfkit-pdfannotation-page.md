

- PDFKit
- PDFAnnotation
-  page 

Instance Property

# page

Returns the page that the annotation is associated with.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
weak var page: PDFPage? { get set }
```

## Return Value

The PDF page associated with the annotation.

## Discussion

The addAnnotation(_:) method in the `PDFPage` class lets you associate an annotation with a page.

## See Also

### Accessing Information About an Annotation

var modificationDate: Date?

Returns the modification date of the annotation.

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

