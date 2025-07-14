

- ARKit
- ARCoachingOverlayView
-  activatesAutomatically 

Instance Property

# activatesAutomatically

A flag that indicates whether the coaching view activates automatically, depending on the current session state.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@MainActor
var activatesAutomatically: Bool { get set }
```

## Discussion

The default value is true. If enabled, the coaching overlay sets isActive automatically, depending on whether it needs user intervention to meet the current goal. The coaching overlay activates when the session is initializing or when tracking conditions have degraded past a certain threshold.

## See Also

### Activating the View

var isActive: Bool

A flag that indicates whether coaching is in progress.

func setActive(Bool, animated: Bool)

Controls whether coaching is in progress.

