

- UIKit
- UITab
-  UITab.Placement 

Enumeration

# UITab.Placement

A tab’s placement when displayed in contexts that allow different placement.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
enum Placement
```

## Topics

### Placement values

case automatic

The system adds only top-level items to the tab bar, but people can add, remove, or move this item.

case `default`

The item appears in the tab bar, but people can move or remove it.

case fixed

The item appears in the tab bar’s leading edge, and people can’t move or remove it.

case movable

The item appears in the tab bar, people can move it but can’t remove it.

case optional

The item doesn’t appear in the tab bar, but people can add it and move it.

case pinned

The item appears as a pinned tab, on the trailing edge of the tab bar.

case sidebarOnly

The item only appears in the sidebar.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing customization

var isHidden: Bool

A Boolean value that indicates whether an item is hidden in a sidebar.

var isHiddenByDefault: Bool

A Boolean value that indicates whether an item is hidden by default.

var allowsHiding: Bool

A Boolean value that indicates whether people can hide a tab in a sidebar.

var preferredPlacement: UITab.Placement

The preferred placement for a tab when displayed in contexts that allow different placement.

