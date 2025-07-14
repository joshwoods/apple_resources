

- UIKit
- UIMenu
-  UIMenu.Options 

Structure

# UIMenu.Options

Options you use to configure a menu’s appearance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
struct Options
```

## Topics

### Options

static var displayInline: UIMenu.Options

An option indicating the menu displays inline with its parent menu instead of displaying as a submenu.

static var destructive: UIMenu.Options

An option indicating the menu’s appearance represents a destructive action.

static var singleSelection: UIMenu.Options

An option indicating whether the menu and its submenus allow a single menu item that’s in the “on” state.

static var displayAsPalette: UIMenu.Options

An option indicating the menu displays as a row of menu elements for choosing from a collection of items.

### Initializers

init(rawValue: UInt)

Creates a menu options structure from data in an unarchiver.

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

### Creating a menu object

convenience init(title: String, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified values.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, and child elements.

convenience init(title: String, subtitle: String?, image: UIImage?, identifier: UIMenu.Identifier?, options: UIMenu.Options, preferredElementSize: UIMenu.ElementSize, children: [UIMenuElement])

Creates a new menu with the specified title, subtitle, image, identifier, menu options, element size, and child elements.

struct Identifier

Constants you use to identify an app’s standard menus.

init?(coder: NSCoder)

Creates a menu from data in an unarchiver.

