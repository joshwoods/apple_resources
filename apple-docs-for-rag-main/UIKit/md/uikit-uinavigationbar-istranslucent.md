

- UIKit
- UINavigationBar
-  isTranslucent 

Instance Property

# isTranslucent

A Boolean value that indicates whether the navigation bar is translucent.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isTranslucent: Bool { get set }
```

## Discussion

When the navigation bar is translucent, configure the edgesForExtendedLayout and extendedLayoutIncludesOpaqueBars properties of your view controller to display your content underneath the navigation bar.

If the navigation bar doesn’t have a custom background image, or if any pixel of the background image has an alpha value of less than `1.0`, the default value of this property is true. If the background image is completely opaque, the default value of this property is false. If you set this property to true and the custom background image is completely opaque, UIKit applies a system-defined opacity of less than `1.0` to the image. If you set this property to false and the background image is not opaque, UIKit adds an opaque backdrop.

## See Also

### Customizing the bar’s appearance

var prefersLargeTitles: Bool

A Boolean value that indicates whether the title displays in a large format.

var standardAppearance: UINavigationBarAppearance

The appearance settings for a standard-height navigation bar.

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for the navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

Legacy customizations

Customize appearance information directly on the navigation bar object.

