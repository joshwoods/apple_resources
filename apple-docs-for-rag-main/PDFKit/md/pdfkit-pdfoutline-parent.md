

- PDFKit
- PDFOutline
-  parent 

Instance Property

# parent

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var parent: PDFOutline? { get }
```

## See Also

### Getting Information About an Outline

var document: PDFDocument?

Returns the document with which the outline is associated.

var numberOfChildren: Int

Returns the number of child outline objects in the outline.

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

var index: Int

Returns the index of the outline.

