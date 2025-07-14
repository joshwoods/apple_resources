

- AppKit
-  NSMenuItem 

Class

# NSMenuItem

A command item in an app menu.

macOS

``` source
class NSMenuItem
```

## Overview

The NSMenuItem class includes some private functionality needed to maintain binary compatibility with other components of Cocoa. Because of this fact, you can’t replace the NSMenuItem class with a different class, but you can subclass it if necessary.

## Topics

### Creating a menu item

init(title: String, action: Selector?, keyEquivalent: String)

Returns an initialized instance of `NSMenuItem`.

init(coder: NSCoder)

### Enabling a menu item

var isEnabled: Bool

A Boolean value that indicates whether the menu item is enabled.

### Managing hidden status

var isHidden: Bool

A Boolean value that indicates whether the menu item is hidden.

var isHiddenOrHasHiddenAncestor: Bool

A Boolean value that indicates whether the menu item or any of its superitems is hidden.

### Managing the target and action

var target: AnyObject?

The menu item’s target.

var action: Selector?

The menu item’s action-method selector.

### Managing the title

var title: String

The menu item’s title.

var attributedTitle: NSAttributedString?

A custom string for a menu item.

### Managing the tag

var tag: Int

The menu item’s tag.

### Managing the state

var state: NSControl.StateValue

The state of the menu item.

### Managing the image

var image: NSImage?

The menu item’s image.

var onStateImage: NSImage!

The image of the menu item that indicates an “on” state.

var offStateImage: NSImage?

The image of the menu item that indicates an “off” state.

var mixedStateImage: NSImage!

The image of the menu item that indicates a “mixed” state, that is, a state neither “on” nor “off.”

### Managing the badge

var badge: NSMenuItemBadge?

### Managing the section header

var isSectionHeader: Bool

A Boolean value indicating whether the menu item is a section header.

### Managing submenus

var submenu: NSMenu?

The submenu of the menu item.

var hasSubmenu: Bool

A Boolean value that indicates whether the menu item has a submenu.

var parent: NSMenuItem?

The menu item whose submenu contains the receiver.

### Managing the separator item

var isSeparatorItem: Bool

A Boolean value indicating whether the menu item is a separator item.

class func separator() -> NSMenuItem

Returns a menu item that is used to separate logical groups of menu commands.

### Managing the owning menu

var menu: NSMenu?

The menu item’s menu.

### Managing key equivalents

var keyEquivalent: String

The menu item’s unmodified key equivalent.

var keyEquivalentModifierMask: NSEvent.ModifierFlags

The menu item’s keyboard equivalent modifiers.

### Managing mnemonics

func setTitleWithMnemonic(String)

Sets the title of a menu item with a character denoting an access key.

Deprecated

### Managing user key equivalents

class var usesUserKeyEquivalents: Bool

Returns a Boolean value that indicates whether menu items conform to user preferences for key equivalents.

var userKeyEquivalent: String

The user-assigned key equivalent for the menu item.

var allowsAutomaticKeyEquivalentLocalization: Bool

A Boolean value that determines whether the system automatically remaps the keyboard shortcut to support localized keyboards.

var allowsAutomaticKeyEquivalentMirroring: Bool

A Boolean value that determines whether the system automatically swaps input strings for some keyboard shortcuts when the interface direction changes.

var allowsKeyEquivalentWhenHidden: Bool

### Managing alternates

var isAlternate: Bool

A Boolean value that marks the menu item as an alternate to the previous menu item.

### Managing indentation levels

var indentationLevel: Int

The menu item indentation level for the menu item.

### Managing tool tips

var toolTip: String?

A help tag for the menu item.

### Representing an object

var representedObject: Any?

The object represented by the menu item.

### Managing the view

var view: NSView?

The content view for the menu item.

### Getting highlighted status

var isHighlighted: Bool

A Boolean value that indicates whether the menu item should be drawn highlighted.

### Identifying the Continuity Camera menu item

class let importFromDeviceIdentifier: NSUserInterfaceItemIdentifier

The identifier for a Continuity Camera menu item, which takes pictures or scans documents using an iOS device.

### Type Methods

static func sectionHeader(title: String) -> NSMenuItem

static func sectionHeader(withTitle: String) -> NSMenuItemDeprecated

### Instance Properties

var subtitle: String?

### Type Properties

class var writingToolsItems: [NSMenuItem]

An array of standard menu items related to Writing Tools. Each call to this method returns an array of newly allocated instances of NSMenuItem.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSCoding
- NSCopying
- NSObjectProtocol
- NSUserInterfaceItemIdentification
- NSValidatedUserInterfaceItem

## See Also

### Menus

class NSMenu

An object that manages an app’s menus.

class NSMenuItemBadge

A control that provides additional quantitative information specific to a menu item, such as the number of available updates.

protocol NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

