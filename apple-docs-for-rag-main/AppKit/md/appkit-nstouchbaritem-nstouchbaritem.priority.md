

- AppKit
- NSTouchBarItem
-  NSTouchBarItem.Priority 

Structure

# NSTouchBarItem.Priority

Priorities for the visibility of a Touch Bar item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
struct Priority
```

## Discussion

Use these constants to set the visibilityPriority property of an NSTouchBarItem instance. The Touch Bar hides items of lower priority when there isn’t enough space to show all items.

## Topics

### Priorities

static let low: NSTouchBarItem.Priority

A constant indicating a low visibility priority.

static let normal: NSTouchBarItem.Priority

A constant indicating a normal visibility priority.

static let high: NSTouchBarItem.Priority

A constant indicating a high visibility priority.

### Initializers

init(Float)

Creates a new priority structure from the given value.

init(rawValue: Float)

Creates a new priority structure from the given raw value.

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

### Managing item visibility

var visibilityPriority: NSTouchBarItem.Priority

Determines which items are shown in a bar when space is limited.

var isVisible: Bool

A Boolean value that reflects whether or not the item is visible.

