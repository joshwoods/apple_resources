

- PDFKit
- PDFView
-  clearSelection() 

Instance Method

# clearSelection()

Clears the selection.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func clearSelection()
```

## Discussion

The view redraws as necessary but does not scroll. This call is equivalent to calling `[PDFView setCurrentSelection:NULL].`

## See Also

### Handling Selections

var currentSelection: PDFSelection?

The current selection.

func setCurrentSelection(PDFSelection?, animate: Bool)

Sets the current selection, in an animated way, if desired.

func selectAll(Any?)

Selects all text in the document.

func copy(Any?)

Copies the text in the selection, if any, to the Pasteboard.

func scrollSelectionToVisible(Any?)

Scrolls the view until the selection is visible.

var highlightedSelections: [PDFSelection]?

Returns the array of selections that are highlighted using `setHighlightedSelections`.

