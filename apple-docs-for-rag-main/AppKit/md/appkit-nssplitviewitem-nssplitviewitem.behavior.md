

- AppKit
- NSSplitViewItem
-  NSSplitViewItem.Behavior 

Enumeration

# NSSplitViewItem.Behavior

Constants that describe the behavior of the split view item.

macOS 10.11+

``` source
enum Behavior
```

## Topics

### Item Behaviors

case `default`

The default split view item behavior.

case sidebar

The sidebar behavior.

case contentList

The content list behavior.

case inspector

The inspector behavior.

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

### Getting the Item Behavior

var behavior: NSSplitViewItem.Behavior

The standard behavior type of the split view item.

