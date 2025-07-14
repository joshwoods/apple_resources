

- AppKit
- NSStandardKeyBindingResponding
-  deleteWordBackward(\_:) 

Instance Method

# deleteWordBackward(\_:)

Deletes the word preceding the current insertion point.

macOS

``` source
@MainActor
optional func deleteWordBackward(_ sender: Any?)
```

## Discussion

If the insertion point is in the middle of a word, this method deletes only the portion of the word preceding the insertion point.

## See Also

### Deleting Content

func deleteBackward(Any?)

Deletes content moving backward from the current insertion point.

func deleteBackwardByDecomposingPreviousCharacter(Any?)

func deleteForward(Any?)

func deleteToBeginningOfLine(Any?)

Deletes content from the insertion point to the beginning of the current line.

func deleteToBeginningOfParagraph(Any?)

Deletes content from the insertion point to the beginning of the current paragraph.

func deleteToEndOfLine(Any?)

Deletes content from the insertion point to the end of the current line.

func deleteToEndOfParagraph(Any?)

Deletes content from the insertion point to the end of the current paragraph.

func deleteWordForward(Any?)

func yank(Any?)

Deletes the current selection, placing it in a temporary buffer, such as the Clipboard.

