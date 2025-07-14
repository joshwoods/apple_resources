

- PDFKit
- PDFOutline
-  document 

Instance Property

# document

Returns the document with which the outline is associated.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
weak var document: PDFDocument? { get }
```

## See Also

### Getting Information About an Outline

var numberOfChildren: Int

Returns the number of child outline objects in the outline.

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

var index: Int

Returns the index of the outline.

