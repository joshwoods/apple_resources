

- Finder Sync
-  FIMenuKind 

Enumeration

# FIMenuKind

The different kinds of custom menus that the Finder Sync extension can provide.

macOS 10.10+

``` source
enum FIMenuKind
```

## Topics

### Constants

case contextualMenuForItems

A shortcut menu created when the user control-clicks on an item or a group of selected items inside the Finder window.

case contextualMenuForContainer

A shortcut menu created when the user control-clicks on the Finder window’s background.

case contextualMenuForSidebar

A shortcut menu created when the user control-clicks on an item in the sidebar.

case toolbarItemMenu

A menu created when the user clicks on the extension’s toolbar button.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

