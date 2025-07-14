

- UIKit
- UIButton
-  isHeld 

Instance Property

# isHeld

A Boolean value that indicates whether the button menu is visible.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@MainActor
var isHeld: Bool { get }
```

## Discussion

The property is true if the button is presenting a menu in response to a long press. Buttons that set showsMenuAsPrimaryAction to present a menu don’t set this property.

## See Also

### Supporting menu and toggle buttons

var menu: UIMenu?

A menu that the button displays.

var changesSelectionAsPrimaryAction: Bool

A Boolean value that indicates whether the button tracks a selection, either through a menu or a toggle.

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

