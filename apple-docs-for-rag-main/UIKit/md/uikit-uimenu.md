

- UIKit
-  UIMenu 

Class

# UIMenu

A container for grouping related menu elements in an app menu or contextual menu.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIMenu
```

## Overview

Create UIMenu objects and use them to construct the menus and submenus your app displays. You provide menus for your app when it runs on macOS, and key command elements in those menus also appear in the discoverability HUD on iPad when someone presses the Command key. You also use menus to display contextual actions in response to specific interactions with one of your views. Every menu has a title, an optional image, and an optional set of child elements. When someone selects an element from the menu, the system executes the code you provide. The code sample below illustrates adding a menu group that contains two menu elements — New and Open — to the File menu.

```
// Ensure that the builder is modifying the menu bar system.
guard builder.system == UIMenuSystem.main else { return }

let newDocument = UIKeyCommand(title: "New",
                               action: #selector(newDocument(_:)),
                               input: "n",
                               modifierFlags: .command)

let openDocument = UIKeyCommand(title: "Open...",
                                action: #selector(openDocument(_:)),
                                input: "o",
                                modifierFlags: .command)

// Use the .displayInline option to avoid displaying the menu as a submenu,
// and to separate it from the other menu elements using a line separator.
let newMenu = UIMenu(title: "", options: .displayInline, children: [newDocument, openDocument])

// Insert the menu item at the top of the File menu.
builder.insertChild(newMenu, atStartOfMenu: .file)
```

For examples of how you use UIMenu, see Adding menus and shortcuts to the menu bar and user interface.

## Topics

### Creating a menu object

convenience init(title: String, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified values.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, and child elements.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, preferredElementSize: UIMenu.ElementSize, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, element size, and child elements.

struct Identifier

Constants you use to identify an app’s standard menus.

struct Options

Options you use to configure a menu’s appearance.

init?(coder: NSCoder)

Creates a menu from data in an unarchiver.

### Accessing child elements

var children: [UIMenuElement]

The contents of the menu.

func replacingChildren([UIMenuElement]) -> UIMenu

Creates a new menu with the same configuration as the current menu, but with a new set of child elements.

### Accessing selected elements

var selectedElements: [UIMenuElement]

The elements in the menu and its sub-menus that are in the on state.

### Getting menu details

var identifier: UIMenu.Identifier

The unique identifier for the current menu.

var options: UIMenu.Options

The configuration options for the current menu.

### Specifying size of menu elements

var preferredElementSize: UIMenu.ElementSize

The size of the menu’s child elements.

enum ElementSize

Constants that determine the size of an element in a menu.

### Customizing menu display

var displayPreferences: UIMenuDisplayPreferences?

An object that configures how UIKit displays the menu.

class UIMenuDisplayPreferences

An object that contains information for configuring a menu’s display.

## Relationships

### Inherits From

- UIMenuElement

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- Sendable
- UIAccessibilityIdentification

## See Also

### App menus

protocol UIMenuBuilder

An interface for adding and removing menus from a menu system.

class UIMenuSystem

An object representing a main or contextual menu system.

