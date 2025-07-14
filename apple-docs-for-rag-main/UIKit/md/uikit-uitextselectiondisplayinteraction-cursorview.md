

- UIKit
- UITextSelectionDisplayInteraction
-  cursorView 

Instance Property

# cursorView

The view that draws the caret at the text insertion point.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var cursorView: any UIView & UITextCursorView { get set }
```

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

When you install the interaction on your text input view, the system installs a view in this property that provides the standard system appearance for the caret at the insertion point. You can replace this view with a custom one you provide to change the appearance of the caret.

## See Also

### Getting the system selection views

var highlightView: any UIView &amp; UITextSelectionHighlightView

The view that draws the selection highlight behind the rendered text.

var handleViews: [any UIView &amp; UITextSelectionHandleView]

The view that draws the selection handles for the selected text.

