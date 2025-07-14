

- UIKit
- UIButton
-  changesSelectionAsPrimaryAction 

Instance Property

# changesSelectionAsPrimaryAction

A Boolean value that indicates whether the button tracks a selection, either through a menu or a toggle.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 17.0+visionOS 1.0+

``` source
@MainActor
var changesSelectionAsPrimaryAction: Bool { get set }
```

## Discussion

This behavior of this property composes with showsMenuAsPrimaryAction and the menu property.

If menu is `nil`, setting this property to true makes the button toggle its selected state.

If you set a menu and showsMenuAsPrimaryAction is false, setting this property to true makes the button a toggle button. The menu functions as a contextual menu, which appears after a long press.

If you set a menu and showsMenuAsPrimaryAction is true, setting this property to true makes the button function as a pop-up. The button presents the menu on touch, the menu tracks the selection in its selectedElements property, and the button title updates to reflect the selection.

## See Also

### Supporting menu and toggle buttons

var menu: UIMenu?

A menu that the button displays.

var isHeld: Bool

A Boolean value that indicates whether the button menu is visible.

var preferredMenuElementOrder: UIContextMenuConfiguration.ElementOrder

The preferred menu-element ordering strategy for the menu.

