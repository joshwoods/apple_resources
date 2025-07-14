

- PDFKit
- PDFView
-  setCurrentSelection(\_:animate:) 

Instance Method

# setCurrentSelection(\_:animate:)

Sets the current selection, in an animated way, if desired.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func setCurrentSelection(
    _ selection: PDFSelection?,
    animate: Bool
)
```

## Discussion

This method behaves as `setCurrentSelection(_:)`, but with the addition of animation, if `animate` is true. The animation serves to draw the user’s attention to the new selection, which can be useful when implementing search.

## See Also

### Handling Selections

var currentSelection: PDFSelection?

The current selection.

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

