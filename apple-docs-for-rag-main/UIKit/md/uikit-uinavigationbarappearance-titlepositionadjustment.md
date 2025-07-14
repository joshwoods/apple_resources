

- UIKit
- UINavigationBarAppearance
-  titlePositionAdjustment 

Instance Property

# titlePositionAdjustment

The distance, in points, by which to offset the title horizontally and vertically.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var titlePositionAdjustment: UIOffset { get set }
```

## Discussion

Positive values move the title down and to the right. Negative values move the title up and to the left.

## See Also

### Configuring the title

var titleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of a standard-size title.

var largeTitleTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of a large-size title.

