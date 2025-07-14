

- UIKit
- UIEditMenuInteractionDelegate
-  editMenuInteraction(\_:willDismissMenuFor:animator:) 

Instance Method

# editMenuInteraction(\_:willDismissMenuFor:animator:)

Informs the delegate when the interaction is about to dismiss the menu.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
optional func editMenuInteraction(
    _ interaction: UIEditMenuInteraction,
    willDismissMenuFor configuration: UIEditMenuConfiguration,
    animator: any UIEditMenuInteractionAnimating
)
```

## Parameters 

`interaction`  

The interaction object triggering the menu.

`configuration`  

The object containing the configuration details for the menu.

`animator`  

The object you use to add animations that run alongside the dismiss transition.

## See Also

### Customizing the Menu

func editMenuInteraction(UIEditMenuInteraction, menuFor: UIEditMenuConfiguration, suggestedActions: [UIMenuElement]) -> UIMenu?

Provides the menu to use when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, targetRectFor: UIEditMenuConfiguration) -> CGRect

Provides the target rectangle to position the menu relative to when the interaction begins or requires an update.

func editMenuInteraction(UIEditMenuInteraction, willPresentMenuFor: UIEditMenuConfiguration, animator: any UIEditMenuInteractionAnimating)

Informs the delegate when the interaction is about to present the menu.

protocol UIEditMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with menus.

