

- SwiftUI
- ScrollTransitionConfiguration
-  animated(\_:) 

Type Method

# animated(\_:)

Creates a new configuration that discretely animates the transition when the view becomes visible.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func animated(_ animation: Animation = .default) -> ScrollTransitionConfiguration
```

## Parameters 

`animation`  

The animation to use when transitioning between states.

## Return Value

A configuration that discretely animates between transition phases.

## Discussion

Unlike the interactive configuration, the transition isn’t interpolated as the scroll view is scrolled. Instead, the transition phase only changes once the threshold has been reached, at which time the given animation is used to animate to the new phase.

## See Also

### Getting the configuration

static let identity: ScrollTransitionConfiguration

Creates a new configuration that does not change the appearance of the view.

static let animated: ScrollTransitionConfiguration

Creates a new configuration that discretely animates the transition when the view becomes visible.

static let interactive: ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

static func interactive(timingCurve: UnitCurve) -> ScrollTransitionConfiguration

Creates a new configuration that interactively interpolates the transition’s effect as the view is scrolled into the visible region of the container.

