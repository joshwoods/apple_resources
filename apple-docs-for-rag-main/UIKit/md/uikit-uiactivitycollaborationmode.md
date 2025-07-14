

- UIKit
-  UIActivityCollaborationMode 

Enumeration

# UIActivityCollaborationMode

A value that defines how the system shares an item.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
enum UIActivityCollaborationMode
```

## Topics

### Enumeration Cases

case collaborate

The system allows collaboration on a shared item.

case sendCopy

The system sends a copy of the item.

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

### Restricting the sharing mode

class CollaborationModeRestriction

An object that disables the sharing mode and optionally displays an alert.

