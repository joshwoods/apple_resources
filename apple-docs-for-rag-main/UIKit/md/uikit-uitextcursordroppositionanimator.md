

- UIKit
-  UITextCursorDropPositionAnimator 

Class

# UITextCursorDropPositionAnimator

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
class UITextCursorDropPositionAnimator
```

## Topics

### Initializers

init!(textCursorView: (any UIView &amp; UITextCursorView)!, textInput: (any UIView &amp; UITextInput)!)

### Instance Properties

var cursorView: (any UIView &amp; UITextCursorView)!

var textInput: (any UIView &amp; UITextInput)!

### Instance Methods

func animate(alongsideChanges: (() -> Void)?, completion: (() -> Void)?)

func placeCursor(at: UITextPosition!, animated: Bool)

func setCursorVisible(Bool, animated: Bool)

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Custom text selection

Adopting system selection UI in custom text views

Incorporate the system text-selection experience into your custom text UI in UIKit.

class UITextSelectionDisplayInteraction

An object that provides the system UI for displaying text selection.

protocol UITextSelectionHighlightView

An interface you use to provide a custom highlight UI behind the selected text.

protocol UITextSelectionHandleView

An interface you use to draw custom the selection handles for ranges of text.

protocol UITextCursorView

An interface you use to draw the insertion point in a piece of text.

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

