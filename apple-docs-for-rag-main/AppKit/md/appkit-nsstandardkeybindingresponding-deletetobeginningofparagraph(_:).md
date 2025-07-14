

- AppKit
- NSStandardKeyBindingResponding
-  deleteToBeginningOfParagraph(\_:) 

Instance Method

# deleteToBeginningOfParagraph(\_:)

Deletes content from the insertion point to the beginning of the current paragraph.

macOS

``` source
@MainActor
optional func deleteToBeginningOfParagraph(_ sender: Any?)
```

## See Also

### Deleting Content

func deleteBackward(Any?)

Deletes content moving backward from the current insertion point.

func deleteBackwardByDecomposingPreviousCharacter(Any?)

func deleteForward(Any?)

func deleteToBeginningOfLine(Any?)

Deletes content from the insertion point to the beginning of the current line.

func deleteToEndOfLine(Any?)

Deletes content from the insertion point to the end of the current line.

func deleteToEndOfParagraph(Any?)

Deletes content from the insertion point to the end of the current paragraph.

func deleteWordBackward(Any?)

Deletes the word preceding the current insertion point.

func deleteWordForward(Any?)

func yank(Any?)

Deletes the current selection, placing it in a temporary buffer, such as the Clipboard.

