

- SwiftUI
- ScrollTransitionConfiguration
-  animation(\_:) 

Instance Method

# animation(\_:)

Sets the animation with which the transition will be applied.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func animation(_ animation: Animation) -> ScrollTransitionConfiguration
```

## Parameters 

`animation`  

An animation that will be used to apply the transition to the view.

## Return Value

A copy of this configuration with the animation set to the given value.

## Discussion

If the transition is interactive, the given animation will be used to animate the effect toward the current interpolated value, causing the effect to lag behind the current scroll position.

## See Also

### Accessing the configuration

func threshold(ScrollTransitionConfiguration.Threshold) -> ScrollTransitionConfiguration

Sets the threshold at which the view will be considered fully visible.

struct Threshold

Describes a specific point in the progression of a target view within a container from hidden (fully outside the container) to visible.

