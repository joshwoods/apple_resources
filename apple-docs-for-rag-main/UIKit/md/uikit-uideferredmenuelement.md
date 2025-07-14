

- UIKit
-  UIDeferredMenuElement 

Class

# UIDeferredMenuElement

A placeholder menu element that the system replaces with the result of the block’s completion handler.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
class UIDeferredMenuElement
```

## Topics

### Creating a deferred menu element

convenience init((([UIMenuElement]) -> Void) -> Void)

A convenience initializer that creates a placeholder menu element that the system replaces with the result of the provider’s completion handler.

class func uncached((([UIMenuElement]) -> Void) -> Void) -> Self

Returns a placeholder menu element that the system replaces with the result of the provider’s completion handler.

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

struct Attributes

Attributes that determine the style of the menu element.

enum State

Constants that indicate the state of an action- or command-based menu element.

protocol UIMenuLeaf

An interface for an object that represents a menu element without child elements.

