

- UIKit
-  UICommand 

Class

# UICommand

A menu element that performs its action in a selector.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UICommand
```

## Overview

Create a UICommand object when you want a menu element that performs its action in a selector available in the responder chain.

```
// Create a selector-based action to use as a menu element.
let refreshCommand = UICommand(title: "Refresh", action: #selector(refreshData(_:)))

// Use the .displayInline option to avoid displaying the menu as a submenu,
// and to separate it from the other menu elements using a line separator.
let refreshMenuItem = UIMenu(title: "", options: .displayInline, children: [refreshCommand])

// Insert the menu into the File menu before the Close menu.
builder.insertSibling(refreshMenuItem, beforeMenu: .close)
```

## Topics

### Creating a command

convenience init(title: String, subtitle: String?, image: UIImage?, action: Selector, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

Creates a command with the specified title, subtitle, image, action, property list, alternative commands, discoverability title, attributes, and state.

convenience init(title: String, image: UIImage?, action: Selector, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

Creates a command with the specified title, image, action, property list, alternative commands, discoverability title, attributes, and state.

init?(coder: NSCoder)

Creates a command from data in an unarchiver.

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

### Getting information about the command

var title: String

The command’s title.

var image: UIImage?

The command’s image.

var action: Selector

The selector identifying the action method called after the user selects the command.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the command.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the command.

var state: UIMenuElement.State

The state of the command.

### Getting command alternatives

var alternates: [UICommandAlternate]

An array of alternative actions to take for the command.

class UICommandAlternate

An object representing an alternative action for a command.

### Associating data

var propertyList: Any?

An object that contains data to associate with the command.

let UICommandTagShare: String

A value that identifies a command as a Share menu.

### Initializers

convenience init(title: String, subtitle: String?, image: UIImage?, selectedImage: UIImage?, action: Selector, propertyList: Any?, alternates: [UICommandAlternate], discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State)

## Relationships

### Inherits From

- UIMenuElement

### Inherited By

- UIKeyCommand

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
- UIMenuLeaf

## See Also

### Menu elements and keyboard shortcuts

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Adopting menus and UIActions in your user interface

Add menus to your user interface, with built-in button support and bar-button items, and create custom menu experiences.

class UIMenuElement

An object representing a menu, action, or command.

class UIAction

A menu element that performs its action in a closure.

class UIKeyCommand

An object that specifies a key press perform on a hardware keyboard and the resulting action.

class UIDeferredMenuElement

A placeholder menu element that the system replaces with the result of the block’s completion handler.

struct Attributes

Attributes that determine the style of the menu element.

enum State

Constants that indicate the state of an action- or command-based menu element.

protocol UIMenuLeaf

An interface for an object that represents a menu element without child elements.

