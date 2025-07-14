

- SwiftUI
-  ToolbarItemPlacement 

Structure

# ToolbarItemPlacement

A structure that defines the placement of a toolbar item.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ToolbarItemPlacement
```

## Overview

There are two types of placements:

- Semantic placements, such as principal and navigation, denote the intent of the item being added. SwiftUI determines the appropriate placement for the item based on this intent and its surrounding context, like the current platform.

- Positional placements, such as navigationBarLeading, denote a precise placement for the item, usually for a particular platform.

In iOS, iPadOS, and macOS, the system uses the space available to the toolbar when determining how many items to render in the toolbar. If not all items fit in the available space, an overflow menu may be created and remaining items placed in that menu.

## Topics

### Getting semantic placement

static let automatic: ToolbarItemPlacement

The system places the item automatically, depending on many factors including the platform, size class, or presence of other items.

static let principal: ToolbarItemPlacement

The system places the item in the principal item section.

static let status: ToolbarItemPlacement

The item represents a change in status for the current context.

### Getting placement for specific actions

static let primaryAction: ToolbarItemPlacement

The item represents a primary action.

static let secondaryAction: ToolbarItemPlacement

The item represents a secondary action.

static let confirmationAction: ToolbarItemPlacement

The item represents a confirmation action for a modal interface.

static let cancellationAction: ToolbarItemPlacement

The item represents a cancellation action for a modal interface.

static let destructiveAction: ToolbarItemPlacement

The item represents a destructive action for a modal interface.

static let navigation: ToolbarItemPlacement

The item represents a navigation action.

### Getting explicit placement

static var topBarLeading: ToolbarItemPlacement

Places the item in the leading edge of the top bar.

static var topBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the top bar.

static let bottomBar: ToolbarItemPlacement

Places the item in the bottom toolbar.

static let bottomOrnament: ToolbarItemPlacement

Places the item in an ornament under the window.

static let keyboard: ToolbarItemPlacement

The item is placed in the keyboard section.

static func accessoryBar&lt;ID>(id: ID) -> ToolbarItemPlacement

Creates a unique accessory bar placement.

### Deprecated symbols

init&lt;ID>(id: ID)

Creates a custom accessory bar item placement.

Deprecated

static let navigationBarLeading: ToolbarItemPlacement

Places the item in the leading edge of the navigation bar.

Deprecated

static let navigationBarTrailing: ToolbarItemPlacement

Places the item in the trailing edge of the navigation bar.

Deprecated

## See Also

### Populating a toolbar

func toolbar(content:)

Populates the toolbar or navigation bar with the specified items.

struct ToolbarItem

A model that represents an item which can be placed in the toolbar or navigation bar.

struct ToolbarItemGroup

A model that represents a group of `ToolbarItem`s which can be placed in the toolbar or navigation bar.

protocol ToolbarContent

Conforming types represent items that can be placed in various locations in a toolbar.

struct ToolbarContentBuilder

Constructs a toolbar item set from multi-expression closures.

