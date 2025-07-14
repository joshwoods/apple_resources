

- UIKit
- UIMenuElement
-  UIMenuElement.Attributes 

Structure

# UIMenuElement.Attributes

Attributes that determine the style of the menu element.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Attributes
```

## Topics

### Attributes

static var destructive: UIMenuElement.Attributes

An attribute indicating the destructive style.

static var disabled: UIMenuElement.Attributes

An attribute indicating the disabled style.

static var hidden: UIMenuElement.Attributes

An attribute indicating the hidden style.

static var keepsMenuPresented: UIMenuElement.Attributes

An attribute indicating that the menu remains presented after firing the element’s action instead of dismissing.

### Initializers

init(rawValue: UInt)

Creates a menu-element attributes structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

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

class UICommand

A menu element that performs its action in a selector.

class UIKeyCommand

An object that specifies a key press perform on a hardware keyboard and the resulting action.

class UIDeferredMenuElement

A placeholder menu element that the system replaces with the result of the block’s completion handler.

enum State

Constants that indicate the state of an action- or command-based menu element.

protocol UIMenuLeaf

An interface for an object that represents a menu element without child elements.

