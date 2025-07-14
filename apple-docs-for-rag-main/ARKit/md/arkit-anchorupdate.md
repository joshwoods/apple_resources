

- ARKit
-  AnchorUpdate 

Structure

# AnchorUpdate

Information about the event that updated an anchor.

visionOS 1.0+

``` source
struct AnchorUpdate where AnchorType : Anchor
```

## Topics

### Inspecting anchor updates

let anchor: AnchorType

The anchor that this anchor update contains information about.

var timestamp: TimeInterval

The time when this anchor update occurred.

let event: AnchorUpdate&lt;AnchorType>.Event

The event which caused the anchor to update.

enum Event

An event that indicates whether an anchor was added, updated, or removed.

var description: String

A textual representation of this anchor update.

## Relationships

### Conforms To

- CustomStringConvertible
- Sendable

## See Also

### Tracking anchors over time

struct AnchorUpdateSequence

An asynchronous sequence of updates to anchors.

