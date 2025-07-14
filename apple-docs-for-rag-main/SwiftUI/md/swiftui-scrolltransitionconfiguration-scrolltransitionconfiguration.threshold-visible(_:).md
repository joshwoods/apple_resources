

- SwiftUI
- ScrollTransitionConfiguration
- ScrollTransitionConfiguration.Threshold
-  visible(\_:) 

Type Method

# visible(\_:)

The target view is visible by the given amount, where zero is fully hidden, and one is fully visible.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static func visible(_ amount: Double) -> ScrollTransitionConfiguration.Threshold
```

## Discussion

Values less than zero or greater than one are clamped.

## See Also

### Getting the threshold

static var centered: ScrollTransitionConfiguration.Threshold

The target view is centered within the container

static let hidden: ScrollTransitionConfiguration.Threshold

static let visible: ScrollTransitionConfiguration.Threshold

