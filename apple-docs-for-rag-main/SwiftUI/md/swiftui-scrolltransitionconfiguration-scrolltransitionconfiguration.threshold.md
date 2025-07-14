

- SwiftUI
- ScrollTransitionConfiguration
-  ScrollTransitionConfiguration.Threshold 

Structure

# ScrollTransitionConfiguration.Threshold

Describes a specific point in the progression of a target view within a container from hidden (fully outside the container) to visible.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct Threshold
```

## Topics

### Getting the threshold

static var centered: ScrollTransitionConfiguration.Threshold

The target view is centered within the container

static let hidden: ScrollTransitionConfiguration.Threshold

static let visible: ScrollTransitionConfiguration.Threshold

static func visible(Double) -> ScrollTransitionConfiguration.Threshold

The target view is visible by the given amount, where zero is fully hidden, and one is fully visible.

### Modifying the threshold

func inset(by: Double) -> ScrollTransitionConfiguration.Threshold

Returns a threshold that is met when the target view is closer to the center of the container by `distance`. Use negative values to move the threshold away from the center.

func interpolated(towards: ScrollTransitionConfiguration.Threshold, amount: Double) -> ScrollTransitionConfiguration.Threshold

Creates a new threshold that combines this threshold value with another threshold, interpolated by the given amount.

## See Also

### Accessing the configuration

func animation(Animation) -> ScrollTransitionConfiguration

Sets the animation with which the transition will be applied.

func threshold(ScrollTransitionConfiguration.Threshold) -> ScrollTransitionConfiguration

Sets the threshold at which the view will be considered fully visible.

