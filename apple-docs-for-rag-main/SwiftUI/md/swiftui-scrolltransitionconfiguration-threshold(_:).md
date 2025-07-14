

- SwiftUI
- ScrollTransitionConfiguration
-  threshold(\_:) 

Instance Method

# threshold(\_:)

Sets the threshold at which the view will be considered fully visible.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func threshold(_ threshold: ScrollTransitionConfiguration.Threshold) -> ScrollTransitionConfiguration
```

## Parameters 

`threshold`  

The threshold specifying how much of the view must intersect with the container before it is treated as visible.

## Return Value

A copy of this configuration with the threshold set to the given value.

## See Also

### Accessing the configuration

func animation(Animation) -> ScrollTransitionConfiguration

Sets the animation with which the transition will be applied.

struct Threshold

Describes a specific point in the progression of a target view within a container from hidden (fully outside the container) to visible.

