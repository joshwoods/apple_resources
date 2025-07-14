

- AppKit
-  NSMenuItemBadge 

Class

# NSMenuItemBadge

A control that provides additional quantitative information specific to a menu item, such as the number of available updates.

macOS 14.0+

``` source
class NSMenuItemBadge
```

## Overview

You create a badge using an initializer or a predefined factory method, and then you assign it to the badge property of a NSMenuItem for display.

For example, to display a badge with a count, use the init(count:) initalizer, passing in the value of `count` as an `Int`.

- Swift
- Objective-C

```
let menu = NSMenu()

// Create a menu item.
let menuItem = NSMenuItem(title: "Messages", action: nil, keyEquivalent: "")

// Set the badge to display "6".
menuItem.badge = NSMenuItemBadge(count: 6)

// Add the item to the menu.
menu.addItem(menuItem)
```

```
NSMenu *menu = [[NSMenu alloc] init];

// Create a menu item.
NSMenuItem *menuItem = [[NSMenuItem alloc] initWithTitle:@"Messages" action:nil keyEquivalent:@""];

// Set the badge to display "6".
menuItem.badge = [[NSMenuItemBadge alloc] initWithCount:6];

// Add the item to the menu.
[menu addItem:menuItem];
```

To display a badge with a custom string, use the init(string:) initializer, passing in the string you want to display.

- Swift
- Objective-C

```
let updateCount = 3
let menu = NSMenu()

// Create a menu item.
let menuItem = NSMenuItem(title: "Changes", action: nil, keyEquivalent: "")

// Set the badge to display "3 changes".
menuItem.badge = NSMenuItemBadge(string: "\(updateCount) changes")

// Add the item to the menu.
menu.addItem(menuItem)
```

```
NSInteger updateCount = 3;
NSMenu *menu = [[NSMenu alloc] init];

// Create a menu item.
NSMenuItem *menuItem = [[NSMenuItem alloc] initWithTitle:@"Changes" action:nil keyEquivalent:@""];

// Set the badge to display "3 changes".
menuItem.badge = [[NSMenuItemBadge alloc] initWithString:[NSString stringWithFormat:@"%ld changes", (long)updateCount]];

// Add the item to the menu.
[menu addItem:menuItem];
```

To display a badge using a predefined NSMenuItemBadge.BadgeType, use a factory method such as newItems(count:), passing in the `count` of the badge to display.

- Swift
- Objective-C

```
let menu = NSMenu()

// Add a new items style badge.
let newItemsItem = NSMenuItem(title: "New Items", action: nil, keyEquivalent: "")
newItemsItem.badge = NSMenuItemBadge.newItems(count: 3)
menu.addItem(newItemsItem)

// Add an alerts style badge.
let alertsItem = NSMenuItem(title: "Alerts", action: nil, keyEquivalent: "")
alertsItem.badge = NSMenuItemBadge.alerts(count: 4)
menu.addItem(alertsItem)

// Add an update style badge.
let updatesItem = NSMenuItem(title: "Updates", action: nil, keyEquivalent: "")
updatesItem.badge = NSMenuItemBadge.updates(count: 5)
menu.addItem(updatesItem)
```

```
NSMenu *menu = [[NSMenu alloc] init];

// Add a new items style badge.
NSMenuItem *newItemsItem = [[NSMenuItem alloc] initWithTitle:@"New Items" action:nil keyEquivalent:@""];
newItemsItem.badge = [NSMenuItemBadge newItemsWithCount:3];
[menu addItem:newItemsItem];

// Add an alerts style badge.
NSMenuItem *alertsItem = [[NSMenuItem alloc] initWithTitle:@"New Items" action:nil keyEquivalent:@""];
alertsItem.badge = [NSMenuItemBadge alertsWithCount:4];
[menu addItem:alertsItem];

// Add an update style badge.
NSMenuItem *updatesItem = [[NSMenuItem alloc] initWithTitle:@"Updates" action:nil keyEquivalent:@""];
updatesItem.badge = [NSMenuItemBadge updatesWithCount:5];
[menu addItem:updatesItem];
```

Important

If you use one of the predefined badge types, the system localizes and pluralizes the string for you. If you create your own custom badge string, you need to localize and pluralize that string yourself. For more information on how to localize and pluralize text, see Localizing and varying text with a string catalog.

The default value of this property is `nil`.

## Topics

### Creating menu item badges

init(count: Int)

Creates a badge with a count and an empty string.

init(string: String)

Creates a badge with the provided custom string.

### Creating badges of a specific type

class func alerts(count: Int) -> Self

Creates an alert-style badge with an integer count and a predefined label that represents the number of alerts.

class func newItems(count: Int) -> Self

Creates a new item-style badge with an integer count and a predefined label that represents the number of new items.

class func updates(count: Int) -> Self

Creates an update-style badge with an integer count and a predefined label that represents the number of available updates.

enum BadgeType

Constants that define types of badges for display.

### Accessing menu item badge attributes

var itemCount: Int

The number of items the badge displays.

var stringValue: String?

The string representation of the badge when it displays.

var type: NSMenuItemBadge.BadgeType

The type of items the badge displays.

### Instance Properties

var stringValue: String?

The string representation of the badge as it would appear when the badge is displayed.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Menus

class NSMenu

An object that manages an app’s menus.

class NSMenuItem

A command item in an app menu.

protocol NSMenuDelegate

The optional methods implemented by delegates of NSMenu objects to manage menu display and handle some events.

