

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:willDisplayMenuFor:animator:) 

Instance Method

# contextMenuInteraction(\_:willDisplayMenuFor:animator:)

Informs the delegate when a menu display begins.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    willDisplayMenuFor configuration: UIContextMenuConfiguration,
    animator: (any UIContextMenuInteractionAnimating)?
)
```

## Parameters 

`interaction`  

The interaction object that triggered the interaction.

`configuration`  

The context menu configuration.

`animator`  

The animator to configure custom animations.

## See Also

### Handling animations

func contextMenuInteraction(UIContextMenuInteraction, willEndFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display ends.

protocol UIContextMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with context menus.

