

- PDFKit
- PDFView
-  scrollSelectionToVisible(\_:) 

Instance Method

# scrollSelectionToVisible(\_:)

Scrolls the view until the selection is visible.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@IBAction @MainActor
func scrollSelectionToVisible(_ sender: Any?)
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

var highlightedSelections: [PDFSelection]?

Returns the array of selections that are highlighted using `setHighlightedSelections`.

