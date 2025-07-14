

- ARKit
- AnchorUpdate
-  event 

Instance Property

# event

The event which caused the anchor to update.

visionOS 1.0+

``` source
let event: AnchorUpdate.Event
```

## See Also

### Inspecting anchor updates

let anchor: AnchorType

The anchor that this anchor update contains information about.

var timestamp: TimeInterval

The time when this anchor update occurred.

enum Event

An event that indicates whether an anchor was added, updated, or removed.

var description: String

A textual representation of this anchor update.

