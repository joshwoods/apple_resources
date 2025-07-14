

- SwiftUI
-  ToolbarItemGroup 

Structure

# ToolbarItemGroup

A model that represents a group of `ToolbarItem`s which can be placed in the toolbar or navigation bar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ToolbarItemGroup where Content : View
```

## Topics

### Creating a toolbar item group

init(placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item group with a specified placement and content.

init&lt;C, L>(placement: ToolbarItemPlacement, content: () -> C, label: () -> L)

Creates a toolbar item group with the specified placement, content, and a label describing that content.

### Supporting types

struct LabeledToolbarItemGroupContent

A view that represents the view of a toolbar item group with a specified label.

## Relationships

### Conforms To

- ToolbarContent

## See Also

### Populating a toolbar

func toolbar(content:)

Populates the toolbar or navigation bar with the specified items.

struct ToolbarItem

A model that represents an item which can be placed in the toolbar or navigation bar.

struct ToolbarItemPlacement

A structure that defines the placement of a toolbar item.

protocol ToolbarContent

Conforming types represent items that can be placed in various locations in a toolbar.

struct ToolbarContentBuilder

Constructs a toolbar item set from multi-expression closures.

