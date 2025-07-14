

- UIKit
-  UIMenuSystem 

Class

# UIMenuSystem

An object representing a main or contextual menu system.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIMenuSystem
```

## Overview

A menu system groups root menus together. The main system has only one root menu while the context system can have multiple root menus, each built in different UIResponder objects like a view controller.

Use UIMenuSystem in your implementation of buildMenu(with:) to isolate changes to a specific system.

```
override func buildMenu(with builder: UIMenuBuilder) {
    super.buildMenu(with: builder)

    // Ensure that the builder is modifying the menu bar system.
    guard builder.system == UIMenuSystem.main else { return }

    // ...
}
```

You can also use a menu system to rebuild or revalidate menus as changes occur in your app. To rebuild a menu, call the setNeedsRebuild() method. Call setNeedsRevalidate() when you need the menu system to revalidate a menu.

For more information, see Adding menus and shortcuts to the menu bar and user interface.

## Topics

### Getting a menu system

class var main: UIMenuSystem

The main menu system.

class var context: UIMenuSystem

The context menu system.

### Rebuilding a menu system

func setNeedsRebuild()

Tells the menu system to rebuild all of its menus.

### Revalidating a menu system

func setNeedsRevalidate()

Tells the menu system to validate all of its menus.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### App menus

class UIMenu

A container for grouping related menu elements in an app menu or contextual menu.

protocol UIMenuBuilder

An interface for adding and removing menus from a menu system.

