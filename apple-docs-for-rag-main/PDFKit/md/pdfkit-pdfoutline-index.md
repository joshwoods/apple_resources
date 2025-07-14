

- PDFKit
- PDFOutline
-  index 

Instance Property

# index

Returns the index of the outline.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
var index: Int { get }
```

## Discussion

The index of the outline object is relative to its siblings and from the perspective of the parent of the outline object. The root outline object, and any outline object without a parent, has an index value of `0`.

## See Also

### Getting Information About an Outline

var document: PDFDocument?

Returns the document with which the outline is associated.

var numberOfChildren: Int

Returns the number of child outline objects in the outline.

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

