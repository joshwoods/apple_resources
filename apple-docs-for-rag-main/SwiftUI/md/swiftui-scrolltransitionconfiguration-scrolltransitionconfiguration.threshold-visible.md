

- SwiftUI
- ScrollTransitionConfiguration
- ScrollTransitionConfiguration.Threshold
-  visible 

Type Property

# visible

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static let visible: ScrollTransitionConfiguration.Threshold
```

## See Also

### Getting the threshold

static var centered: ScrollTransitionConfiguration.Threshold

The target view is centered within the container

static let hidden: ScrollTransitionConfiguration.Threshold

static func visible(Double) -> ScrollTransitionConfiguration.Threshold

The target view is visible by the given amount, where zero is fully hidden, and one is fully visible.

