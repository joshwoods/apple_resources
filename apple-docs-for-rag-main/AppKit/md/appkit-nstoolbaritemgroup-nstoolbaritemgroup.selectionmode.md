

- AppKit
- NSToolbarItemGroup
-  NSToolbarItemGroup.SelectionMode 

Enumeration

# NSToolbarItemGroup.SelectionMode

A value that indicates how a grouped toolbar item selects its subitems.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
enum SelectionMode
```

## Topics

### Selection modes

case momentary

The system temporarily highlights the select group item when the user selects the item.

case selectAny

The system toggles a highlight on any item selected.

case selectOne

The system displays a highlighted mode on the most recent item selected.

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

### Items

class NSToolbarItem

A single item that appears in a window’s toolbar.

class NSToolbarItemGroup

A group of subitems in a toolbar item.

enum ControlRepresentation

class NSMenuToolbarItem

A control that presents a menu in a window’s toolbar.

class NSSearchToolbarItem

A toolbar item that contains a search field optimized for performing text-based searches.

class NSTrackingSeparatorToolbarItem

A toolbar separator that aligns with the vertical split view in the same window.

