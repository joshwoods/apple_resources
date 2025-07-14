

- UIKit
- UIContextMenuInteractionDelegate
-  contextMenuInteraction(\_:willEndFor:animator:) 

Instance Method

# contextMenuInteraction(\_:willEndFor:animator:)

Informs the delegate when a menu display ends.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
optional func contextMenuInteraction(
    _ interaction: UIContextMenuInteraction,
    willEndFor configuration: UIContextMenuConfiguration,
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

func contextMenuInteraction(UIContextMenuInteraction, willDisplayMenuFor: UIContextMenuConfiguration, animator: (any UIContextMenuInteractionAnimating)?)

Informs the delegate when a menu display begins.

protocol UIContextMenuInteractionAnimating

Methods adopted by system-supplied animator objects when interacting with context menus.

