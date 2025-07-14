

- UIKit
-  UITextSelectionHighlightView 

Protocol

# UITextSelectionHighlightView

An interface you use to provide a custom highlight UI behind the selected text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UITextSelectionHighlightView : UICoordinateSpace
```

## Overview

Adopt the UITextSelectionHighlightView protocol in a custom view you use to draw the highlight behind text in one of your text views. Use your custom view in conjunction with a UITextSelectionDisplayInteraction object to apply your custom selection UI to one of your text views. This protocol provides the rectangles for your view to fill with the highlight color and appearance. Use CALayer objects or your view’s draw(_:) method to draw these rectangles.

After adopting this protocol in your custom view, assign your view to the highlightView property of the interaction object you attached to your text view.

## Topics

### Getting the rectangles to draw

var selectionRects: [UITextSelectionRect]

The rectangles to draw with the selection highlight.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol
- UICoordinateSpace

## See Also

### Custom text selection

Adopting system selection UI in custom text views

Incorporate the system text-selection experience into your custom text UI in UIKit.

class UITextSelectionDisplayInteraction

An object that provides the system UI for displaying text selection.

protocol UITextSelectionHandleView

An interface you use to draw custom the selection handles for ranges of text.

protocol UITextCursorView

An interface you use to draw the insertion point in a piece of text.

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextCursorDropPositionAnimator

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

