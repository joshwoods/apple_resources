

- AppKit
- NSTouch
-  identity 

Instance Property

# identity

The changes to a particular touch during its lifetime.

macOS 10.6+

``` source
var identity: any NSCopying & NSObjectProtocol { get }
```

## Discussion

While touch identities may be re-used, they are unique during the life of the touch, even when multiple devices are present.

Identity objects implement the NSCopying protocol so that they may be used as keys in an NSDictionary. Use isEqual: to compare two touch identities.

## See Also

### Using Touch Properties

var phase: NSTouch.Phase

The current phase of the touch.

struct Phase

The possible phases of a touch.

var normalizedPosition: NSPoint

The normalized position of the touch.

var isResting: Bool

The indicator for a resting touch.

