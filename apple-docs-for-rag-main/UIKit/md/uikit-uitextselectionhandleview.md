

- UIKit
-  UITextSelectionHandleView 

Protocol

# UITextSelectionHandleView

An interface you use to draw custom the selection handles for ranges of text.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
protocol UITextSelectionHandleView : UICoordinateSpace
```

## Overview

Adopt the UITextSelectionHandleView protocol in a custom view you use to draw text-selection handles in one of your text views. Use your custom view in conjunction with a UITextSelectionDisplayInteraction object to apply your custom selection UI to one of your text views. This protocol provides the preferred frame for the selection handle, and you provide details about the handle back to the system. Use CALayer objects or your view’s draw(_:) method to draw the handles.

After adopting this protocol in your custom view, create exactly two instances and assign them to the handleViews property of the interaction object you attached to your text view. Configure one instance as the leading selection handle, and configure the other instance as the trailing selection handle.

## Topics

### Providing the preferred frame rectangle

func preferredFrame(for: CGRect) -> CGRect

**Required**

### Specifying the handle details

var direction: NSDirectionalRectEdge

The orientation of the selection handle.

**Required**

var customShape: UIBezierPath?

The custom shape to draw for the stem of the selection handle.

**Required**

var isVertical: Bool

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

protocol UITextSelectionHighlightView

An interface you use to provide a custom highlight UI behind the selected text.

protocol UITextCursorView

An interface you use to draw the insertion point in a piece of text.

class UIStandardTextCursorView

A view that draws the standard system insertion point in a piece of text.

class UITextCursorDropPositionAnimator

class UITextLoupeSession

An object that manages the presentation of the system magnifier at the location you specify.

