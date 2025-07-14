

- AppKit
- NSMenu
-  NSMenu.SelectionMode 

Enumeration

# NSMenu.SelectionMode

Describes how the menu manages selection states of the menu items that belong to the same selection group.

macOS 14.0+

``` source
enum SelectionMode
```

## Overview

This doesn’t apply to menu items that have distinct target-action values.

## Topics

### Defining the selection mode

case automatic

A selection mode where the menu determines the appropriate selection mode based on the context and its constants.

case selectAny

A selection mode where someone can select multiple items in the menu.

case selectOne

A selection mode where someone can select at most one menu item in the same selection group at the same time.

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

### Selecting Items

var selectedItems: [NSMenuItem]

The menu items that are currently selected.

var selectionMode: NSMenu.SelectionMode

The selection mode of the menu.

