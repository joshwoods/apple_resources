

- AppKit
-  NSToolbarItemGroup 

Class

# NSToolbarItemGroup

A group of subitems in a toolbar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.5+

``` source
@MainActor
class NSToolbarItemGroup
```

## Overview

An NSToolbarItemGroup represents a collection set of subitems in a toolbar that the system displays based on available space and settings that you specify. The system uses the views and labels of the subitems, but the parent’s attributes take precedence. This differs from other NSToolbarItem objects because they’re attached — the user drags them together as a single item rather than separately.

If a subitem of the group has an action set on it, the group uses that action instead of its own when the user clicks or taps on that item. The system prefers the subitem’s action if it exists, otherwise it uses the group’s action.

To configure an instance of NSToolbarItemGroup, you first create the individual toolbar subitems:

```
NSToolbarItem *item1 = [[NSToolbarItem alloc] initWithItemIdentifier:@"Item1"];
NSToolbarItem *item2 = [[NSToolbarItem alloc] initWithItemIdentifier:@"Item2"];
[item1 setImage:[NSImage imageNamed:@"LeftArrow"]];
[item2 setImage:[NSImage imageNamed:@"RightArrow"]];
[item1 setLabel:@"Prev"];
[item2 setLabel:@"Next"];
```

Then, you put them in a grouped item:

```
NSToolbarItemGroup *group = [[NSToolbarItemGroup alloc] initWithItemIdentifier:@"GroupItem"];
[group setSubitems:[NSArray arrayWithObjects:item1, item2, nil]];
```

In this configuration, you get two grouped items, and two labels.

If you set a label on the parent item, you get two grouped items with one shared label:

```
[group setLabel:@"Navigate"];
```

If instead you set a view on the parent item, you get two labels with one shared view:

```
[group setView:someSegmentedControl];
```

## Topics

### Creating grouped toolbar items

convenience init(itemIdentifier: NSToolbarItem.Identifier, images: [UIImage], selectionMode: NSToolbarItemGroup.SelectionMode, labels: [String]?, target: Any?, action: Selector?)

Creates a grouped toolbar item with images.

convenience init(itemIdentifier: NSToolbarItem.Identifier, titles: [String], selectionMode: NSToolbarItemGroup.SelectionMode, labels: [String]?, target: Any?, action: Selector?)

Creates a grouped toolbar item with labels.

### Working with subitems

var subitems: [NSToolbarItem]

The subitems of the grouped toolbar item.

var selectedIndex: Int

The index value for the most recently selected subitem of a grouped toolbar item.

func isSelected(at: Int) -> Bool

Indicates whether a specified index is currently selected.

func setSelected(Bool, at: Int)

Sets the selected state of a subitem in a grouped toolbar item.

### Configuring grouped toolbar items

var controlRepresentation: NSToolbarItemGroup.ControlRepresentation

A value that represents how a toolbar displays a grouped toolbar item.

enum ControlRepresentation

var selectionMode: NSToolbarItemGroup.SelectionMode

The selection mode of the grouped toolbar item.

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

## Relationships

### Inherits From

- NSToolbarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSMenuItemValidation
- NSObjectProtocol
- NSValidatedUserInterfaceItem
- Sendable

## See Also

### Items

class NSToolbarItem

A single item that appears in a window’s toolbar.

enum ControlRepresentation

enum SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

