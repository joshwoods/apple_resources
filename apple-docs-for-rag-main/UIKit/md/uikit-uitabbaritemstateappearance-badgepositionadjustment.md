

- UIKit
- UITabBarItemStateAppearance
-  badgePositionAdjustment 

Instance Property

# badgePositionAdjustment

The additional amount by which to offset the badge horizontally and vertically.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var badgePositionAdjustment: UIOffset { get set }
```

## Discussion

Use this property to specify the distance, in points, by which to offset the badge from its default position over its item. Positive values move the title down and to the right. Negative values move the title up and to the left.

## See Also

### Configuring the badge appearance

var badgeTextAttributes: [NSAttributedString.Key : Any]

String attributes to apply to the text of the item’s badge.

var badgeBackgroundColor: UIColor?

The background color of the badge.

var badgeTitlePositionAdjustment: UIOffset

The additional amount by which to offset the badge’s title horizontally and vertically.

