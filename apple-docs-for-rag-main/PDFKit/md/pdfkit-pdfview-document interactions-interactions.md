

- PDFKit
- PDFView
-  Document Interactions 

API Collection

# Document Interactions

Handle selections, work with annotation actions, convert page and view points, and work with mouse events in a document.

## Topics

### Handling Selections

var currentSelection: PDFSelection?

The current selection.

func setCurrentSelection(PDFSelection?, animate: Bool)

Sets the current selection, in an animated way, if desired.

func selectAll(Any?)

Selects all text in the document.

func clearSelection()

Clears the selection.

func copy(Any?)

Copies the text in the selection, if any, to the Pasteboard.

func scrollSelectionToVisible(Any?)

Scrolls the view until the selection is visible.

var highlightedSelections: [PDFSelection]?

Returns the array of selections that are highlighted using `setHighlightedSelections`.

### Working with Annotation Actions

func annotationsChanged(on: PDFPage)

Tells the PDF view that an annotation on the specified page has changed.

Link Annotations

Validate and handle links in a PDF view.

### Converting Page and View Points

func page(for: CGPoint, nearest: Bool) -> PDFPage?

Returns the page containing a point specified in view coordinates.

func convert(CGPoint, to: PDFPage) -> CGPoint

Converts a point from view space to page space.

func convert(CGRect, to: PDFPage) -> CGRect

Converts a rectangle from view space to page space.

func convert(CGPoint, from: PDFPage) -> CGPoint

Converts a point from page space to view space.

func convert(CGRect, from: PDFPage) -> CGRect

Converts a rectangle from page space to view space.

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

Drag Operations

Define drag operations allowed for a view.

