

- UIKit
- UITabBarItemStateAppearance
-  badgeTextAttributes 

Instance Property

# badgeTextAttributes

String attributes to apply to the text of the item’s badge.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var badgeTextAttributes: [NSAttributedString.Key : Any] { get set }
```

## Discussion

If you don’t specify font or color attributes for the text, UIKit supplies appropriate default values. For a list of possible keys, see NSAttributedString.Key.

## See Also

### Configuring the badge appearance

var badgeBackgroundColor: UIColor?

The background color of the badge.

var badgeTitlePositionAdjustment: UIOffset

The additional amount by which to offset the badge’s title horizontally and vertically.

var badgePositionAdjustment: UIOffset

The additional amount by which to offset the badge horizontally and vertically.

