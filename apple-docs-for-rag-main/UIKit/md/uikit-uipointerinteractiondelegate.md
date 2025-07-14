

- UIKit
-  UIPointerInteractionDelegate 

Protocol

# UIPointerInteractionDelegate

An interface for handling pointer movements within the interaction’s view.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
protocol UIPointerInteractionDelegate : NSObjectProtocol
```

## Topics

### Defining pointer styles for regions

func pointerInteraction(UIPointerInteraction, regionFor: UIPointerRegionRequest, defaultRegion: UIPointerRegion) -> UIPointerRegion?

Asks the delegate for a region as the pointer moves within the interaction’s view.

func pointerInteraction(UIPointerInteraction, styleFor: UIPointerRegion) -> UIPointerStyle?

Asks the delegate for a pointer style after an interaction receives a new region.

### Handling animations for pointer regions

func pointerInteraction(UIPointerInteraction, willEnter: UIPointerRegion, animator: any UIPointerInteractionAnimating)

Informs the delegate when the pointer enters a given region.

func pointerInteraction(UIPointerInteraction, willExit: UIPointerRegion, animator: any UIPointerInteractionAnimating)

Informs the delegate when the pointer exits a given region.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Essentials

class UIPointerInteraction

An interaction that enables support for effects on a view or customizes the pointer’s appearance within a region of an app.

Integrating pointer interactions into your iPad app

Support touch interactions in your iPad app by adding pointer interactions to your views.

Enhancing your iPad app with pointer interactions

Provide a great user experience with pointing devices, by incorporating pointer content effects and shape customizations.

