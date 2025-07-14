

- UIKit
-  UIMenuElement 

Class

# UIMenuElement

An object representing a menu, action, or command.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIMenuElement
```

## Overview

UIMenuElement defines the behavior shared by all menus, actions, and commands. You don’t create UIMenuElement objects directly. Instead, you create an appropriate object that inherits from this class, such as UIMenu, UIAction, or UICommand.

## Topics

### Getting the element attributes

var title: String

The title of the menu element.

var subtitle: String?

The subtitle to display alongside the menu element’s title.

var image: UIImage?

The image to display alongside the menu element’s title.

### Creating a menu element

init?(coder: NSCoder)

Creates a menu element from data in an unarchiver.

### Constants

struct Attributes

Attributes that determine the style of the menu element.

enum State

Constants that indicate the state of an action- or command-based menu element.

## Relationships

### Inherits From

- NSObject

### Inherited By

- UIAction
- UICommand
- UIDeferredMenuElement
- UIMenu

### Conforms To

- CVarArg
- Copyable
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

### Menu elements and keyboard shortcuts

Adding menus and shortcuts to the menu bar and user interface

Provide quick access to useful actions by adding menus and keyboard shortcuts to your Mac app built with Mac Catalyst.

Adopting menus and UIActions in your user interface

Add menus to your user interface, with built-in button support and bar-button items, and create custom menu experiences.

class UIAction

A menu element that performs its action in a closure.

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

