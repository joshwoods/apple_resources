

- BrowserEngineKit
- BETextInput
-  automaticallyPresentEditMenu 

Instance Property

# automaticallyPresentEditMenu

Controls whether the edit menu is allowed to be presented or should be suppressed.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
var automaticallyPresentEditMenu: Bool { get }
```

**Required**

## See Also

### Editing and correcting text

func transposeCharactersAroundSelection()

Transposes the characters on either side of the caret in response to the key command, ctrl + T

**Required**

func replaceText(String, withText: String, options: BETextReplacementOptions, completionHandler: ([UITextSelectionRect]) -> Void)

Replace the specified text preceding the current selection.

**Required**

func requestTextContextForAutocorrection(completionHandler: (BETextDocumentContext) -> Void)

Invoked by the system to gather context around the current selection. Clients should generally include the setence that contains the current selection and include the previous sentence if the current selection is at a boundary.

**Required**

func requestTextRects(for: String, withCompletionHandler: ([UITextSelectionRect]) -> Void)

Invoked by the system to gather context for the presentation of various text related UI’s. Completion handler should be invoked with the `UITextSelectionRect`s for the substring nearest to the caret that matches the given `input`

**Required**

func requestPreferredArrowDirectionForEditMenu(completionHandler: (UIEditMenuArrowDirection) -> Void)

Invoked by the system to gather context, including the client’s preference for how the edit menu should be positioned relative to the selected text.

**Required**

func systemWillPresentEditMenu(withAnimator: any UIEditMenuInteractionAnimating)

Invoked by the system when it is about to present an edit menu with an animator.

**Required**

func systemWillDismissEditMenu(withAnimator: any UIEditMenuInteractionAnimating)

Invoked by the system when it is about to dismiss an edit menu with an animator.

**Required**

