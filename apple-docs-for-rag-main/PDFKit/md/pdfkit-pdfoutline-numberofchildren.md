

- PDFKit
- PDFOutline
-  numberOfChildren 

Instance Property

# numberOfChildren

Returns the number of child outline objects in the outline.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
var numberOfChildren: Int { get }
```

## See Also

### Getting Information About an Outline

var document: PDFDocument?

Returns the document with which the outline is associated.

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

var index: Int

Returns the index of the outline.

