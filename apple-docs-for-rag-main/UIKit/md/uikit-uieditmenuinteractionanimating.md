

- UIKit
-  UIEditMenuInteractionAnimating 

Protocol

# UIEditMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with menus.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UIEditMenuInteractionAnimating : NSObjectProtocol
```

## Topics

### Adding Animations

func addAnimations(() -> Void)

Adds a closure that performs animations to run alongside the edit menu interaction presentation.

**Required**

func addCompletion(() -> Void)

Adds a closure to perform operations when the edit menu interaction presentation animations are complete.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the Menu

func editMenuInteraction(UIEditMenuInteraction, menuFor: UIEditMenuConfiguration, suggestedActions: [UIMenuElement]) -> UIMenu?

Provides the menu to use when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, targetRectFor: UIEditMenuConfiguration) -> CGRect

Provides the target rectangle to position the menu relative to when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, willPresentMenuFor: UIEditMenuConfiguration, animator: any UIEditMenuInteractionAnimating)

Informs the delegate when the interaction is about to present the menu.

func editMenuInteraction(UIEditMenuInteraction, willDismissMenuFor: UIEditMenuConfiguration, animator: any UIEditMenuInteractionAnimating)

Informs the delegate when the interaction is about to dismiss the menu.

