

- PDFKit
- PDFView
-  highlightedSelections 

Instance Property

# highlightedSelections

Returns the array of selections that are highlighted using `setHighlightedSelections`.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var highlightedSelections: [PDFSelection]? { get set }
```

## See Also

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

