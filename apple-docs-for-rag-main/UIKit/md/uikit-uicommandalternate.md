

- UIKit
-  UICommandAlternate 

Class

# UICommandAlternate

An object representing an alternative action for a command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UICommandAlternate
```

## Overview

Create a UICommandAlternate object and add it to a UICommand or UIKeyCommand object when you want to provide users an alternative action for the command. The command alternate is available to the user when they press the keyboard modifier keys, like Control or Option, specified in the modifierFlags property.

For instance, an app may have a Reload menu, created with a key command, that has the keyboard shortcut Command+R. When the user selects Reload, or presses Command+R on their keyboard, the app reloads the data displayed in the current window. The app, however, can display more than one window, so it includes a Reload All alternative for Reload that reloads data in all windows, not just the current one.

The Reload All command alternate specifies alternate in its modifierFlags property, which makes Reload All available to the user when they press the Option key. To select Reload All, the user can press and hold the Option key while displaying the menu that contains Reload. This replaces the Reload menu with Reload All. The user can also select Reload All by pressing Option+Command+R.

```
// Create an alternate for the reload command. The alternative command appears
// in the menu system when the user holds down the keys specified in `modifierFlags`.
let reloadAlternate = UICommandAlternate(title: "Reload All",
                                         action: #selector(reloadAllData(_:)),
                                         modifierFlags: [.alternate])

// Create a selector-based action with a keyboard shortcut to use as a menu element.
let reloadCommand = UIKeyCommand(title: "Reload",
                                action: #selector(reloadData(_:)),
                                input: "r",
                                modifierFlags: [.command],
                                alternates: [reloadAlternate])

// Use the .displayInline option to avoid displaying the menu as a submenu,
// and to separate it from the other menu elements using a line separator.
let reloadMenuItem = UIMenu(title: "", options: .displayInline, children: [reloadCommand])

// Insert the menu into the File menu before the Close menu.
builder.insertSibling(reloadMenuItem, beforeMenu: .close)
```

## Topics

### Creating a command alternative

convenience init(title: String, action: Selector, modifierFlags: UIKeyModifierFlags)

Creates a command alternative with the specified title, action, and modifier flags.

init?(coder: NSCoder)

Creates a command alternative from data in an unarchiver.

### Getting information about the alternative

var title: String

The command alternative’s title.

var action: Selector

The command alternative’s action-method selector.

var modifierFlags: UIKeyModifierFlags

The bit mask of modifier keys that the user must press to invoke the action for the alternative command.

## Relationships

### Inherits From

- NSObject

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

## See Also

### Getting command alternatives

var alternates: [UICommandAlternate]

An array of alternative actions to take for the command.

