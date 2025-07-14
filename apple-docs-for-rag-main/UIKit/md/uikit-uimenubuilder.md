

- UIKit
-  UIMenuBuilder 

Protocol

# UIMenuBuilder

An interface for adding and removing menus from a menu system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
protocol UIMenuBuilder
```

## Mentioned in 

Optimizing your iPad app for Mac

## Overview

You don’t create a menu builder object. Instead, you override buildMenu(with:) in your app delegate or view controller to receive a builder object. Where you override this method determines the system that the builder updates. To add and remove menus from the menu bar using the main menu system, override buildMenu(with:) in your app delegate. To build a context menu using the context system, override the method in your view controller.

To see an example of how to use a menu builder object, see Adding menus and shortcuts to the menu bar and user interface.

## Topics

### Getting menu systems and elements

var system: UIMenuSystem

The menu system that the menu builder modifies.

**Required**

func menu(for: UIMenu.Identifier) -> UIMenu?

Gets the menu for the specified menu identifier.

**Required**

func action(for: UIAction.Identifier) -> UIAction?

Gets the action for the specified action identifier.

**Required**

func command(for: Selector, propertyList: Any?) -> UICommand?

Gets the command for the specified selector and property list.

### Inserting child menus

func insertChild(UIMenu, atStartOfMenu: UIMenu.Identifier)

Adds a child menu as the first element of the specified parent menu.

**Required**

func insertChild(UIMenu, atEndOfMenu: UIMenu.Identifier)

Adds a child menu as the last element of the specified parent menu.

**Required**

### Inserting sibling menus

func insertSibling(UIMenu, beforeMenu: UIMenu.Identifier)

Inserts a sibling menu before the specified menu.

**Required**

func insertSibling(UIMenu, afterMenu: UIMenu.Identifier)

Inserts a sibling menu after the specified menu.

**Required**

### Replacing menus and child menu elements

func replace(menu: UIMenu.Identifier, with: UIMenu)

Replaces the specified menu with a new menu.

**Required**

func replaceChildren(ofMenu: UIMenu.Identifier, from: ([UIMenuElement]) -> [UIMenuElement])

Replaces the elements in a menu with the elements returned by the specified handler block.

**Required**

### Removing a menu

func remove(menu: UIMenu.Identifier)

Removes a menu from the menu system.

**Required**

## See Also

### App menus

class UIMenu

A container for grouping related menu elements in an app menu or contextual menu.

class UIMenuSystem

An object representing a main or contextual menu system.

