

- UIKit
- UIMenu
- UIMenu.Options
-  destructive 

Type Property

# destructive

An option indicating the menu’s appearance represents a destructive action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
static var destructive: UIMenu.Options { get }
```

## Discussion

Apply this option when you need a menu for a destructive action. Use the menu’s title to communicate the action to perform, and use the menu’s child menu elements to ask for user confirmation of that action.

## See Also

### Options

static var displayInline: UIMenu.Options

An option indicating the menu displays inline with its parent menu instead of displaying as a submenu.

static var singleSelection: UIMenu.Options

An option indicating whether the menu and its submenus allow a single menu item that’s in the “on” state.

static var displayAsPalette: UIMenu.Options

An option indicating the menu displays as a row of menu elements for choosing from a collection of items.

