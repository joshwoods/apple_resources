

- WebKit
- WebView
-  replaceSelection(with:) 

Instance Method

# replaceSelection(with:)

Replaces the receiver’s current selection with the specified DOM node.

macOS

``` source
@MainActor
func replaceSelection(with node: DOMNode!)
```

## Parameters 

`node`  

The node that replaces the current selection. If `nil`, a `NOT_FOUND_ERR` DOM error is thrown as an exception. Use the deleteSelection() method to delete the selection.

## Discussion

If the current selection is collapsed (a range is selected with the same nodes and offsets for the start and end) then no content is removed when inserting the node, and the selection is collapsed and moved to the end of the inserted content. If no content is selected, the node is not inserted.

## See Also

### Editing Documents

func replaceSelection(withText: String!)

Replaces the current selection with a string of text.

func replaceSelection(withMarkupString: String!)

Replaces the current selection with mixed text and markup.

func replaceSelection(with: WebArchive!)

Replaces the current selection with an archive’s contents.

func deleteSelection()

Deletes the receiver’s current selection unless it’s collapsed.

func moveToBeginningOfSentence(Any?)

Moves the insertion point to the beginning of the current sentence.

func moveToBeginningOfSentenceAndModifySelection(Any?)

Moves the insertion point and extends the selection to the beginning of the current sentence.

func moveToEndOfSentence(Any?)

Moves the insertion point to the end of the current sentence.

func moveToEndOfSentenceAndModifySelection(Any?)

Moves the insertion point and extends the selection to the end of the current sentence.

func selectSentence(Any?)

Selects the entire sentence around the insertion point.

func toggleContinuousSpellChecking(Any?)

Toggles whether continuous spell checking is available.

func toggleSmartInsertDelete(Any?)

Toggles whether spaces around selected words are inserted or deleted to preserve proper spacing and punctuation.

var canMakeTextStandardSize: Bool

A Boolean that indicates whether the current text size is a multiple of 1.

func makeTextStandardSize(Any?)

Resets the text size to a multiple of 1.

var maintainsInactiveSelection: Bool

A Boolean that indicates whether the selection is maintained when focus is lost.

