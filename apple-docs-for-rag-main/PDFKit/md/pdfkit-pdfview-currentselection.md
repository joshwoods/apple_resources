

- PDFKit
- PDFView
-  currentSelection 

Instance Property

# currentSelection

The current selection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var currentSelection: PDFSelection? { get set }
```

## Discussion

Returns `NULL` if no selection exists.

Note that this method returns the actual instance of the current `PDFSelection` object. Therefore, if you want to modify it, you should make a copy of the returned selection and modify that, instead.

## See Also

### Handling Selections

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

