

- UIKit
- UIPreviewInteraction
-  cancel() 

Instance Method

# cancel()

Cancels the current preview interaction.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func cancel()
```

## Discussion

When a preview interaction is in progress, use this method to cancel it, preventing any further callbacks to the delegate methods.

## See Also

### Handling preview interactions

var view: UIView?

The view from which the preview interaction receives touch events.

func location(in: (any UICoordinateSpace)?) -> CGPoint

Returns the location of the touch that started the interaction.

