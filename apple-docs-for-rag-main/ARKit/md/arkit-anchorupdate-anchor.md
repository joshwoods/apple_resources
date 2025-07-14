

- ARKit
- AnchorUpdate
-  anchor 

Instance Property

# anchor

The anchor that this anchor update contains information about.

visionOS 1.0+

``` source
let anchor: AnchorType
```

## See Also

### Inspecting anchor updates

var timestamp: TimeInterval

The time when this anchor update occurred.

let event: AnchorUpdate&lt;AnchorType>.Event

The event which caused the anchor to update.

enum Event

An event that indicates whether an anchor was added, updated, or removed.

var description: String

A textual representation of this anchor update.

