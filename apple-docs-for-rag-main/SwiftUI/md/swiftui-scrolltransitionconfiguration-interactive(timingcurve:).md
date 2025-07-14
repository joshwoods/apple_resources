

- SwiftUI
- ScrollTransitionConfiguration
-  interactive(timingCurve:) 

Type Method

# interactive(timingCurve:)

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func interactive(timingCurve: UnitCurve = .easeInOut) -> ScrollTransitionConfiguration
```

## Parameters 

`timingCurve`  

The curve that adjusts the pace at which the effect is interpolated between phases of the transition. For example, an `.easeIn` curve causes interpolation to begin slowly as the view reaches the edge of the scroll view, then speed up as it reaches the visible threshold. The curve is applied ‘forward’ while the view is appearing, meaning that time zero corresponds to the view being just hidden, and time 1.0 corresponds to the pont at which the view reaches the configuration threshold. This also means that the timing curve is applied in reversed while the view is moving away from the center of the scroll view.

## Return Value

A configuration that interactively interpolates between transition phases based on the current scroll position.

## See Also

### Getting the configuration

static let identity: ScrollTransitionConfiguration

Creates a new configuration that does not change the appearance of the view.

static let animated: ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static func animated(Animation) -> ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static let interactive: ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

