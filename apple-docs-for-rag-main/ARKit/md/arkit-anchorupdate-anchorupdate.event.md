

- ARKit
- AnchorUpdate
-  AnchorUpdate.Event 

Enumeration

# AnchorUpdate.Event

An event that indicates whether an anchor was added, updated, or removed.

visionOS 1.0+

``` source
@frozen
enum Event
```

## Topics

### Inspecting anchor update events

case added

An event that occurs when ARKit starts tracking an anchor.

case updated

An event that occurs when an existing anchor updates data.

case removed

An event that occurs when ARKit stops tracking an anchor.

### Instance Properties

var description: String

A textual representation of AnchorUpdate.Event

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- CustomStringConvertible
- Equatable
- Hashable
- Sendable

## See Also

### Inspecting anchor updates

let anchor: AnchorType

The anchor that this anchor update contains information about.

var timestamp: TimeInterval

The time when this anchor update occurred.

let event: AnchorUpdate&lt;AnchorType>.Event

The event which caused the anchor to update.

var description: String

A textual representation of this anchor update.

