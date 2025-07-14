

- ARKit
- AnchorUpdate
-  timestamp 

Instance Property

# timestamp

The time when this anchor update occurred.

visionOS 1.0+

``` source
var timestamp: TimeInterval { get }
```

## See Also

### Inspecting anchor updates

let anchor: AnchorType

The anchor that this anchor update contains information about.

let event: AnchorUpdate&lt;AnchorType>.Event

The event which caused the anchor to update.

enum Event

An event that indicates whether an anchor was added, updated, or removed.

var description: String

A textual representation of this anchor update.

