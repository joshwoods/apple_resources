

- UIKit
-  UIAction 

Class

# UIAction

A menu element that performs its action in a closure.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIAction
```

## Overview

Create a UIAction object when you want a menu element that performs its action in a closure. The following example adds an action-based menu to the File menu:

```
// Create a closure-based action to use as a menu element.
let refreshAction = UIAction(title: "Refresh") { (action) in
    print("Refresh the data.")
}

// Use the .displayInline option to avoid displaying the menu as a submenu,
// and to separate it from the other menu elements using a line separator.
let refreshMenuItem = UIMenu(title: "", options: .displayInline, children: [refreshAction])

// Insert the menu into the File menu before the Close menu.
builder.insertSibling(refreshMenuItem, beforeMenu: .close)
```

## Topics

### Creating an action

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, subtitle, image, identifier, discoverability title, attributes, state, and handler.

convenience init(title: String, image: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

Creates an action with the specified title, image, identifier, discoverability title, attributes, state, and handler.

class func captureTextFromCamera(responder: any UIResponder &amp; UIKeyInput, identifier: UIAction.Identifier?) -> Self

Creates an action for capturing text using the device’s camera.

struct Identifier

A type that represents an action identifier.

typealias UIActionHandler

A type that defines the closure for an action handler.

### Getting information about the action

var title: String

The action’s title.

var image: UIImage?

The action’s image.

var identifier: UIAction.Identifier

The unique identifier for the action.

var discoverabilityTitle: String?

An elaborated title that explains the purpose of the action.

var attributes: UIMenuElement.Attributes

The attributes indicating the style of the action.

var state: UIMenuElement.State

The state of the action.

var sender: Any?

The object responsible for the action handler.

### Initializers

convenience init(title: String, subtitle: String?, image: UIImage?, selectedImage: UIImage?, identifier: UIAction.Identifier?, discoverabilityTitle: String?, attributes: UIMenuElement.Attributes, state: UIMenuElement.State, handler: UIActionHandler)

## Relationships

### Inherits From

- UIMenuElement

### Inherited By

- UIWindowScene.ActivationAction

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

class UICommand

A menu element that performs its action in a selector.

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

