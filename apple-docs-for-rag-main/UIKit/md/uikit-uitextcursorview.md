

- UIKit
-  UITextCursorView 

Protocol

# UITextCursorView

An interface you use to draw the insertion point in a piece of text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UITextCursorView : UICoordinateSpace
```

## Overview

Adopt the UITextCursorView protocol in a custom view you use to draw the insertion caret in one of your text views. Use your custom view in conjunction with a UITextSelectionDisplayInteraction object to apply your custom selection UI to one of your text views. This protocol provides details about when to display the blink animations. Use CALayer objects or your view’s draw(_:) method to draw and animate the caret.

After adopting this protocol in your custom view, assign your view to the cursorView property of the interaction object you attached to your text view.

## Topics

### Determining the animation state

var isBlinking: Bool

A Boolean value that determines whether the blink animation is running.

**Required**

func resetBlinkAnimation()

Resets the blink animation to avoid glitches while someone is typing.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UICoordinateSpace

### Conforming Types

- UIStandardTextCursorView

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

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextCursorDropPositionAnimator

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

