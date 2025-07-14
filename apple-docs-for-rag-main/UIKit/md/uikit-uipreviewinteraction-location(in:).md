

- UIKit
- UIPreviewInteraction
-  location(in:) 

Instance Method

# location(in:)

Returns the location of the touch that started the interaction.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func location(in coordinateSpace: (any UICoordinateSpace)?) -> CGPoint
```

## Parameters 

`coordinateSpace`  

The coordinate space in which the touch location should be returned.

## Return Value

The CGPoint that represents the current location of the touch, translated into the requested coordinate space.

## Discussion

Use this method to establish the current location of the touch that triggered the preview interaction.

Note

UIView adopts the UICoordinateSpace protocol, so you can find the touch location within a view in the view hierarchy.

When the preview interaction isn’t running, calling this method returns an invalid point. You must therefore only call this method in response to one of the delegate callbacks specified in UIPreviewInteractionDelegate.

## See Also

### Handling preview interactions

var view: UIView?

The view from which the preview interaction receives touch events.

func cancel()

Cancels the current preview interaction.

