

- UIKit
- UITabBar
-  isTranslucent 

Instance Property

# isTranslucent

A Boolean value that indicates whether the tab bar is translucent.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOS

``` source
@MainActor
var isTranslucent: Bool { get set }
```

## Discussion

When the tab bar is translucent, configure the edgesForExtendedLayout and extendedLayoutIncludesOpaqueBars properties of your view controller to display your content underneath the tab bar.

If the tab bar doesn’t have a custom background image, or if any pixel of the background image has an alpha value of less than `1.0`, the default value of this property is true. If the background image is completely opaque, the default value of this property is false. If you set this property to true and the custom background image is completely opaque, UIKit applies a system-defined opacity of less than `1.0` to the image. If you set this property to false and the background image is not opaque, UIKit adds an opaque backdrop.

## See Also

### Customizing tab bar appearance

var standardAppearance: UITabBarAppearance

The appearance settings for a standard-height tab bar.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var leadingAccessoryView: UIView

The view at the leading edge of a tab bar on tvOS.

var trailingAccessoryView: UIView

The view at the trailing edge of a tab bar on tvOS.

Legacy customizations

Customize appearance information directly on the tab bar object.

