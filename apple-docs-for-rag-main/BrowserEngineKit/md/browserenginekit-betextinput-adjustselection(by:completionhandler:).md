

- BrowserEngineKit
- BETextInput
-  adjustSelection(by:completionHandler:) 

Instance Method

# adjustSelection(by:completionHandler:)

Adjusts the selection by the moving the selected range by the given `range`, in character granularity units.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func adjustSelection(
    by range: BEDirectionalTextRange,
    completionHandler: @escaping () -> Void
)
```

``` source
func adjustSelection(by range: BEDirectionalTextRange) async
```

**Required**

## Discussion

The start of the current selection is moved by `range.offset` characters, and the length of the selection is modified by `range.length` characters. For instance, if the current selection is the word “world” in “Hello world” and the `range` is `{ -6, -2 }`, the selected text after adjustment will be “Hel”.

## See Also

### Selecting text

var selectedText: String?

String representing the selected text.

**Required**

var selectedTextRange: UITextRange?

Range representing the selected text.

**Required**

var isSelectionAtDocumentStart: Bool

Represents whether the current selection is at the beginning of the document

**Required**

func caretRect(for: UITextPosition) -> CGRect

Returns a rectangle to draw the caret at a specified insertion point.

**Required**

func selectionRects(for: UITextRange) -> [UITextSelectionRect]

Returns an array of selection rects corresponding to the range of text.

**Required**

func selectWordForReplacement()

Selects a word with autocorrect replacement suggestions when it is tapped

**Required**

func updateSelection(extent: CGPoint, boundary: UITextGranularity, completionHandler: (Bool) -> Void)

Includes the text up to the given point in the current text selection.

**Required**

func selectText(in: UITextGranularity, at: CGPoint, completionHandler: () -> Void)

Selects the text within the given granularity at the given point in the text view.

**Required**

func selectPosition(at: CGPoint, completionHandler: () -> Void)

Sets the selection caret to the given point

**Required**

func selectPosition(at: CGPoint, for: BETextDocumentRequest, completionHandler: (BETextDocumentContext) -> Void)

Sets the selection caret to the given point. Also includes a convenience document context request.

**Required**

func move(byOffset: Int)

Adjusts the current selection by `offset` in character granularity units

**Required**

func moveSelection(atBoundary: UITextGranularity, in: UITextStorageDirection, completionHandler: () -> Void)

Moves the caret to relative to the current position in the `direction` to the given `granularity`. The `direction` is “forward” or “backward” in accordance with the directionality of the language.

**Required**

func selectTextForEditMenuWithLocation(inView: CGPoint, completionHandler: (Bool, String?, NSRange) -> Void)

Indicates the edit menu is being shown at the given location in the text input view’s coordinate space.

**Required**

