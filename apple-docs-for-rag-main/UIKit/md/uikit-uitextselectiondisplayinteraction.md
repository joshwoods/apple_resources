

- UIKit
-  UITextSelectionDisplayInteraction 

Class

# UITextSelectionDisplayInteraction

An object that provides the system UI for displaying text selection.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
class UITextSelectionDisplayInteraction
```

## Mentioned in 

Adopting system selection UI in custom text views

## Overview

Related sessions from WWDC23

Session 10058: What’s new with text and text interactions

## Topics

### Creating a text selection display interaction

init(textInput: any UITextInput, delegate: any UITextSelectionDisplayInteractionDelegate)

Creates a new text selection display interaction object for the specified text view.

### Managing the drawing view

var delegate: (any UITextSelectionDisplayInteractionDelegate)?

A delegate that provides a container view to manage the system-supplied selection views.

protocol UITextSelectionDisplayInteractionDelegate

An object you use to customize the presentation of text selections in your interface.

### Activating the selection UI

var isActivated: Bool

A Boolean value that indicates whether to display the system selection UI.

### Reporting changes to the selection

func setNeedsSelectionUpdate()

Tells the system to update the selection UI to match the current selection state.

func layoutManagedSubviews()

Loads the selection from the text input view and lays out the selection-related views.

### Getting the text input view

var textInput: (any UITextInput)?

The text input object that manages the selection.

### Getting the system selection views

var highlightView: any UIView &amp; UITextSelectionHighlightView

The view that draws the selection highlight behind the rendered text.

var handleViews: [any UIView &amp; UITextSelectionHandleView]

The view that draws the selection handles for the selected text.

var cursorView: any UIView &amp; UITextCursorView

The view that draws the caret at the text insertion point.

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
- UIInteraction

## See Also

### Custom text selection

Adopting system selection UI in custom text views

Incorporate the system text-selection experience into your custom text UI in UIKit.

protocol UITextSelectionHighlightView

An interface you use to provide a custom highlight UI behind the selected text.

protocol UITextSelectionHandleView

An interface you use to draw custom the selection handles for ranges of text.

protocol UITextCursorView

An interface you use to draw the insertion point in a piece of text.

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextCursorDropPositionAnimator

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

