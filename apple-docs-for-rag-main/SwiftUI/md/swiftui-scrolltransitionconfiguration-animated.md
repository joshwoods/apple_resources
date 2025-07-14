

- SwiftUI
- ScrollTransitionConfiguration
-  animated 

Type Property

# animated

Creates a new configuration that discretely animates the transition when the view becomes visible.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let animated: ScrollTransitionConfiguration
```

## See Also

### Getting the configuration

static let identity: ScrollTransitionConfiguration

Creates a new configuration that does not change the appearance of the view.

static func animated(Animation) -> ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static let interactive: ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

static func interactive(timingCurve: UnitCurve) -> ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

