

- PDFKit
- PDFOutline
-  removeFromParent() 

Instance Method

# removeFromParent()

Removes the outline object from its parent (does nothing if outline object is the root outline object).

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
func removeFromParent()
```

## See Also

### Related Documentation

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

### Changing an Outline Hierarchy

func insertChild(PDFOutline, at: Int)

Inserts the specified outline object at the specified index.

