

- WebKit
- WebView
-  makeTextStandardSize(\_:) 

Instance Method

# makeTextStandardSize(\_:)

Resets the text size to a multiple of 1.

macOS

``` source
@IBAction @MainActor
func makeTextStandardSize(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## See Also

### Editing Documents

func replaceSelection(with: DOMNode!)

Replaces the receiver’s current selection with the specified DOM node.

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

var maintainsInactiveSelection: Bool

A Boolean that indicates whether the selection is maintained when focus is lost.

