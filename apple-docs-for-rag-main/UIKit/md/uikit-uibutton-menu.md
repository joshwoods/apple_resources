

- UIKit
- UIButton
-  menu 

Instance Property

# menu

A menu that the button displays.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 17.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var menu: UIMenu? { get set }
```

## Discussion

The default value is `nil`. When this property changes, the button automatically enables and disables the contextMenuInteraction.

## See Also

### Supporting menu and toggle buttons

var isHeld: Bool

A Boolean value that indicates whether the button menu is visible.

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button tracks a selection, either through a menu or a toggle.

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

