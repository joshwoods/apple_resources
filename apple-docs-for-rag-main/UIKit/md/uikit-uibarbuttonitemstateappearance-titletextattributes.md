

- UIKit
- UIBarButtonItemStateAppearance
-  titleTextAttributes 

Instance Property

# titleTextAttributes

String attributes to apply to the text of the bar button item’s title.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var titleTextAttributes: [NSAttributedString.Key : Any] { get set }
```

## Discussion

If you don’t specify font or color attributes for the text, UIKit supplies appropriate default values. For a list of possible keys, see NSAttributedString.Key.

## See Also

### Configuring the title

var titlePositionAdjustment: UIOffset

The additional amount by which to offset the title horizontally and vertically.

