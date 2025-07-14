

- ARKit
- AnchorUpdate
-  description 

Instance Property

# description

A textual representation of this anchor update.

visionOS 1.0+

``` source
var description: String { get }
```

## See Also

### Inspecting anchor updates

let anchor: AnchorType

The anchor that this anchor update contains information about.

var timestamp: TimeInterval

The time when this anchor update occurred.

let event: AnchorUpdate&lt;AnchorType>.Event

The event which caused the anchor to update.

enum Event

An event that indicates whether an anchor was added, updated, or removed.

