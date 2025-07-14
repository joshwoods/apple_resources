

- PDFKit
- PDFView
- Document Interactions
-  Drag Operations 

API Collection

# Drag Operations

Define drag operations allowed for a view.

## Topics

### Dragging in a View

var allowsDragging: Bool

A Boolean value indicating whether the view can accept new PDF documents dragged into it by the user.

Deprecated

var acceptsDraggedFiles: Bool

A Boolean value indicating whether you can drag a file into the view.

## See Also

### Working with Mouse Position and Events

func areaOfInterest(forMouse: UIEvent) -> PDFAreaOfInterest

Returns the type of area the mouse cursor is over.

func areaOfInterest(for: CGPoint) -> PDFAreaOfInterest

Returns the type of area for a specific cursor location point.

struct PDFAreaOfInterest

The mouse position over PDF view areas.

func setCursorFor(PDFAreaOfInterest)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

func perform(PDFAction)

Performs the specified action.

