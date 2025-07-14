

- PDFKit
- PDFOutline
-  insertChild(\_:at:) 

Instance Method

# insertChild(\_:at:)

Inserts the specified outline object at the specified index.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
func insertChild(
    _ child: PDFOutline,
    at index: Int
)
```

## Discussion

To build a PDF outline hierarchy, use this method to add child outline objects. Before you call this method on a `PDFOutline` object that already has a parent, you should retain the object and call removeFromParent() on it first.

## See Also

### Related Documentation

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

### Changing an Outline Hierarchy

func removeFromParent()

Removes the outline object from its parent (does nothing if outline object is the root outline object).

