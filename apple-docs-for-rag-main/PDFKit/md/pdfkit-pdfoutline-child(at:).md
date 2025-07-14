

- PDFKit
- PDFOutline
-  child(at:) 

Instance Method

# child(at:)

Returns the child outline object at the specified index.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
func child(at index: Int) -> PDFOutline?
```

## Discussion

The index is zero-based. This method throws an exception if `index` is out of range.

Important

In macOS 10.5 and later, a `PDFOutline` object retains all its children, so `childAtIndex:` returns the same retained child outline object every time it’s called. This means that you do not need to retain the object returned by `childAtIndex:`. This differs from the behavior of `PDFOutline` in OS X v10.4. In Tiger, `childAtIndex:` returns an auto-released, one-off child outline object, when meant that you had to include code to retain the child.

## See Also

### Getting Information About an Outline

var document: PDFDocument?

Returns the document with which the outline is associated.

var numberOfChildren: Int

Returns the number of child outline objects in the outline.

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

var index: Int

Returns the index of the outline.

