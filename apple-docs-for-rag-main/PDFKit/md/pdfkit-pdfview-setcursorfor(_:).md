

- PDFKit
- PDFView
-  setCursorFor(\_:) 

Instance Method

# setCursorFor(\_:)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

macOS 10.4+

``` source
@MainActor
func setCursorFor(_ area: PDFAreaOfInterest)
```

## Discussion

This method is especially useful for custom subclasses of the `PDFView` class.

## See Also

### Working with Mouse Position and Events

func areaOfInterest(forMouse: UIEvent) -> PDFAreaOfInterest

Returns the type of area the mouse cursor is over.

func areaOfInterest(for: CGPoint) -> PDFAreaOfInterest

Returns the type of area for a specific cursor location point.

struct PDFAreaOfInterest

The mouse position over PDF view areas.

func perform(PDFAction)

Performs the specified action.

Drag Operations

Define drag operations allowed for a view.

