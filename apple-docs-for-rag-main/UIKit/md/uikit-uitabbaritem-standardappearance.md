

- UIKit
- UITabBarItem
-  standardAppearance 

Instance Property

# standardAppearance

The appearance settings for a tab bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var standardAppearance: UITabBarAppearance? { get set }
```

## Discussion

When a tab bar displays the selected item, the appearance setting in this property overrides the settings in the standardAppearance property of UITabBar.

Use this property to apply a tab bar appearance based on the tab bar item stored in the selectedItem property. If the selected item’s standardAppearance property is `nil`, UIKit uses the tab bar’s standard appearance.

## See Also

### Configuring the item’s appearance

var selectedImage: UIImage?

The source image the item uses to generate its selected image.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var titlePositionAdjustment: UIOffset

The offset to apply to the title’s position.

