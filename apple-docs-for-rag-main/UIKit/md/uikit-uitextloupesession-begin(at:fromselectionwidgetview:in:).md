

- UIKit
- UITextLoupeSession
-  begin(at:fromSelectionWidgetView:in:) 

Type Method

# begin(at:fromSelectionWidgetView:in:)

Creates a new loupe session and displays the loupe at the specified location in your view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+tvOS 17.0+

``` source
@MainActor
class func begin(
    at point: CGPoint,
    fromSelectionWidgetView selectionWidget: UIView?,
    in interactionView: UIView
) -> Self?
```

## Parameters 

`point`  

The point in your view’s coordinate system that you want to magnify using the loupe. When creating the loupe with a gesture recognizer, specify the location of the gesture.

`selectionWidget`  

The view associated with the insertion point. When using a UITextSelectionDisplayInteraction object to display selections in your view, specify the view in the interaction object’s cursorView property for this parameter.

`interactionView`  

The view in which to display the loupe. Specify all coordinate values relative to this view.

## Return Value

A new loupe session for the specified view. The method returns `nil` if showing the loupe is inappropriate in the current context.

## Mentioned in 

Adopting system selection UI in custom text views

## Discussion

Call this method to animate the appearance of the loupe at the specified `point` in `interactionView`. Store a strong reference to this returned session and use it to update the position of the loupe. To hide the loupe again, call invalidate() and then remove your reference to the session.

