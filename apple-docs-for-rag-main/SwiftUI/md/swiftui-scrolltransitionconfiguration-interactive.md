

- SwiftUI
- ScrollTransitionConfiguration
-  interactive 

Type Property

# interactive

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let interactive: ScrollTransitionConfiguration
```

## See Also

### Getting the configuration

static let identity: ScrollTransitionConfiguration

Creates a new configuration that does not change the appearance of the view.

static let animated: ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static func animated(Animation) -> ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static func interactive(timingCurve: UnitCurve) -> ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

