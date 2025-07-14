

- UIKit
-  UIInteraction 

Protocol

# UIInteraction

The protocol that an interaction implements to access the view that owns it.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol UIInteraction : NSObjectProtocol
```

## Mentioned in 

Adding Writing Tools support to a custom UIKit view

## Topics

### Getting the View

var view: UIView?

The view that owns the interaction.

**Required**

### Tracking the Movements

func didMove(to: UIView?)

Tells the interaction that a view added or removed it from the view’s interactions array.

**Required**

func willMove(to: UIView?)

Tells the interaction that a view will add or remove it from the view’s interactions array.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- UIBandSelectionInteraction
- UICanvasFeedbackGenerator
- UIContextMenuInteraction
- UIDragInteraction
- UIDropInteraction
- UIEditMenuInteraction
- UIFeedbackGenerator
- UIFindInteraction
- UIImpactFeedbackGenerator
- UIIndirectScribbleInteraction
- UILargeContentViewerInteraction
- UINotificationFeedbackGenerator
- UIPencilInteraction
- UIPointerInteraction
- UIScribbleInteraction
- UISelectionFeedbackGenerator
- UISpringLoadedInteraction
- UITextInteraction
- UITextSelectionDisplayInteraction
- UIToolTipInteraction
- UIWindowScene.ActivationInteraction
- UIWindowSceneDragInteraction
- UIWritingToolsCoordinator

## See Also

### Adding and removing interactions

func addInteraction(any UIInteraction)

Adds an interaction to the view.

func removeInteraction(any UIInteraction)

Removes an interaction from the view.

var interactions: [any UIInteraction]

The array of interactions for the view.

