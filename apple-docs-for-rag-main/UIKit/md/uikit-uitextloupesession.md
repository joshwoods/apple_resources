

- UIKit
-  UITextLoupeSession 

Class

# UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+

``` source
@MainActor
class UITextLoupeSession
```

## Mentioned in 

Adopting system selection UI in custom text views

## Overview

A UITextLoupeSession object programmatically displays the system loupe in your view. You might display this view to allow someone to magnify your view’s content. Typically, you display the loupe from a UIPanGestureRecognizer when someone interacts with your view. As the location in the gesture recognizer changes, use the loupe session object to update the position of the loupe.

## Topics

### Creating the loupe session

class func begin(at: CGPoint, fromSelectionWidgetView: UIView?, in: UIView) -> Self?

Creates a new loupe session and displays the loupe at the specified location in your view.

### Updating the loupe during the session

func move(to: CGPoint, withCaretRect: CGRect, trackingCaret: Bool)

Moves the loupe to the specified point in the session’s associated view.

func invalidate()

Hides the loupe and cleans up any session-related state.

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

class UITextCursorDropPositionAnimator

