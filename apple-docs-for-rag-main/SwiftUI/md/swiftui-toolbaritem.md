

- SwiftUI
-  ToolbarItem 

Structure

# ToolbarItem

A model that represents an item which can be placed in the toolbar or navigation bar.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ToolbarItem where Content : View
```

## Topics

### Creating a toolbar item

init(placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content.

init(id: String, placement: ToolbarItemPlacement, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

init(id: String, placement: ToolbarItemPlacement, showsByDefault: Bool, content: () -> Content)

Creates a toolbar item with the specified placement and content, which allows for user customization.

Deprecated

## Relationships

### Conforms To

- Copyable
- CustomizableToolbarContent

  Conforms when `ID` is `String` and `Content` conforms to `View`.

- Identifiable
- ToolbarContent

## See Also

### Populating a toolbar

func toolbar(content:)

Populates the toolbar or navigation bar with the specified items.

struct ToolbarItemGroup

A model that represents a group of `ToolbarItem`s which can be placed in the toolbar or navigation bar.

struct ToolbarItemPlacement

A structure that defines the placement of a toolbar item.

protocol ToolbarContent

Conforming types represent items that can be placed in various locations in a toolbar.

struct ToolbarContentBuilder

Constructs a toolbar item set from multi-expression closures.

