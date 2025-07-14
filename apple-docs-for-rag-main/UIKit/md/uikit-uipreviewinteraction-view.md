

- UIKit
- UIPreviewInteraction
-  view 

Instance Property

# view

The view from which the preview interaction receives touch events.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
weak var view: UIView? { get }
```

## Discussion

A preview interaction operates on the view that’s provided at initialization time. Use this property to obtain a reference to that same view. Note that this is a weak property — the preview interaction doesn’t retain a reference to the view it’s provided.

## See Also

### Handling preview interactions

func cancel()

Cancels the current preview interaction.

func location(in: (any UICoordinateSpace)?) -> CGPoint

Returns the location of the touch that started the interaction.

