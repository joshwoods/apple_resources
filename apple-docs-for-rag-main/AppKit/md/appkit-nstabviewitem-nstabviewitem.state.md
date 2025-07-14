

- AppKit
- NSTabViewItem
-  NSTabViewItem.State 

Enumeration

# NSTabViewItem.State

These constants describe the current display state of a tab:

macOS

``` source
enum State
```

## Topics

### Constants

case backgroundTab

A tab that’s not being displayed.

case pressedTab

A tab that the user is in the process of clicking. That is, the user has pressed the mouse button while the cursor is over the tab but has not released the mouse button.

case selectedTab

The tab that’s being displayed.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

