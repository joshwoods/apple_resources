

- AppKit
- NSMenu
-  NSMenu.Properties 

Structure

# NSMenu.Properties

These constants are used as a bitmask for specifying a set of menu or menu item properties, and are contained by the propertiesToUpdate property.

macOS

``` source
struct Properties
```

## Topics

### Constants

static var propertyItemTitle: NSMenu.Properties

The menu item’s title.

static var propertyItemAttributedTitle: NSMenu.Properties

The menu item’s attributed string title.

static var propertyItemKeyEquivalent: NSMenu.Properties

The menu item’s key equivalent.

static var propertyItemImage: NSMenu.Properties

The menu image.

static var propertyItemEnabled: NSMenu.Properties

Whether the menu item is enabled or disabled.

static var propertyItemAccessibilityDescription: NSMenu.Properties

The menu item’s accessibility description.

### Creating an NSMenu Property

init(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

