

- UIKit
- UITextSelectionDisplayInteraction
-  handleViews 

Instance Property

# handleViews

The view that draws the selection handles for the selected text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var handleViews: [any UIView & UITextSelectionHandleView] { get set }
```

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

When you install the interaction on your text input view, the system installs two views in this property that provide the standard system appearance for the selection handles. You can replace these views with custom ones you provide to change the appearance of the selection handles.

Important

When assigning a value to this property, you must provide exactly two views. One view provides the leading selection handle and the other provides the trailing selection handle.

## See Also

### Getting the system selection views

var highlightView: any UIView &amp; UITextSelectionHighlightView

The view that draws the selection highlight behind the rendered text.

var cursorView: any UIView &amp; UITextCursorView

The view that draws the caret at the text insertion point.

