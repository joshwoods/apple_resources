

- AppKit
- NSToolbarItem
-  NSToolbarItem.VisibilityPriority 

Structure

# NSToolbarItem.VisibilityPriority

Constants that indicate which toolbar items to keep in the toolbar when space is limited.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
struct VisibilityPriority
```

## Overview

When a toolbar doesn’t have enough space to fit all its items, it pushes items into the overflow menu to make space. Use these constants to suggest a priority for individual toolbar items. The toolbar pushes low-priority items to the overflow menu first, followed by standard items and high-priority items. When two or more items share the same priority, the toolbar pushes the one closest to the trailing edge first.

## Topics

### Visibility priorities

static let standard: NSToolbarItem.VisibilityPriority

The default visibility priority.

static let low: NSToolbarItem.VisibilityPriority

The lowest-priority for a toolbar item.

static let high: NSToolbarItem.VisibilityPriority

A high priority that makes it less likely for the toolbar item to move to the overflow item.

static let user: NSToolbarItem.VisibilityPriority

The highest priority for items in the toolbar.

### Initializers

init(Int)

Creates a visibility priority structure.

init(rawValue: Int)

Creates a visibility priority structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Comparable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the item’s configuration

var isVisible: Bool

A Boolean value that indicates whether the item is currently visible in the toolbar, and not in the overflow menu.

var isBordered: Bool

A Boolean value that indicates whether the toolbar item has a bordered style.

var isNavigational: Bool

A Boolean value that indicates whether the item behaves as a navigation item in the toolbar.

var isEnabled: Bool

A Boolean value that indicates whether the item is enabled.

var allowsDuplicatesInToolbar: Bool

A Boolean value that indicates whether the toolbar item can appear more than once in a toolbar.

Deprecated

var visibilityPriority: NSToolbarItem.VisibilityPriority

The display priority associated with the toolbar item.

var tag: Int

An integer tag you can use to identify the toolbar item.

