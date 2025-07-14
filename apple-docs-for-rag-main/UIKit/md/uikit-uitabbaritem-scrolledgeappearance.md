

- UIKit
- UITabBarItem
-  scrollEdgeAppearance 

Instance Property

# scrollEdgeAppearance

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var scrollEdgeAppearance: UITabBarAppearance? { get set }
```

## Discussion

When a tab bar displays the selected item, the appearance setting in this property overrides the settings in the scrollEdgeAppearance property of UIToolbar.

Use this property to apply a scroll edge appearance based on the tab bar item stored in the selectedItem property. If the selected item’s scrollEdgeAppearance property is `nil`, UIKit uses the tab bar’s scroll edge appearance.

## See Also

### Configuring the item’s appearance

var selectedImage: UIImage?

The source image the item uses to generate its selected image.

var standardAppearance: UITabBarAppearance?

The appearance settings for a tab bar.

var titlePositionAdjustment: UIOffset

The offset to apply to the title’s position.

