

- AppKit
- NSTouch
-  normalizedPosition 

Instance Property

# normalizedPosition

The normalized position of the touch.

macOS 10.6+

``` source
var normalizedPosition: NSPoint { get }
```

## Discussion

The normalized position is a scaled value between (0.0) and (1.0,1.0), where (0.0,0.0) is the lower-left position on the touch device.

## See Also

### Using Touch Properties

var identity: any NSCopying &amp; NSObjectProtocol

The changes to a particular touch during its lifetime.

var phase: NSTouch.Phase

The current phase of the touch.

struct Phase

The possible phases of a touch.

var isResting: Bool

The indicator for a resting touch.

