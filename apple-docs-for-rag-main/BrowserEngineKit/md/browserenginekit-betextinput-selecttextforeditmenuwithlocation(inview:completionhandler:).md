

- BrowserEngineKit
- BETextInput
-  selectTextForEditMenuWithLocation(inView:completionHandler:) 

Instance Method

# selectTextForEditMenuWithLocation(inView:completionHandler:)

Indicates the edit menu is being shown at the given location in the text input view’s coordinate space.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
func selectTextForEditMenuWithLocation(
    inView locationInView: CGPoint,
    completionHandler: @escaping (Bool, String?, NSRange) -> Void
)
```

``` source
func selectTextForEditMenuWithLocation(inView locationInView: CGPoint) async -> (Bool, String?, NSRange)
```

**Required**

## Discussion

The completion handler takes a BOOL indicating whether or not the menu should be shown, a string representing the text context around the updated selection range (generally encompassing the paragraph that contains the selection range) as well as the range of the updated selection, relative to the paragraph context.

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

func adjustSelection(by: BEDirectionalTextRange, completionHandler: () -> Void)

Adjusts the selection by the moving the selected range by the given `range`, in character granularity units.

**Required**

func move(byOffset: Int)

Adjusts the current selection by `offset` in character granularity units

**Required**

func moveSelection(atBoundary: UITextGranularity, in: UITextStorageDirection, completionHandler: () -> Void)

Moves the caret to relative to the current position in the `direction` to the given `granularity`. The `direction` is “forward” or “backward” in accordance with the directionality of the language.

**Required**

