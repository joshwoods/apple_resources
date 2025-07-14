

- UIKit
- UIToolbar
-  isTranslucent 

Instance Property

# isTranslucent

A Boolean value that indicates whether the toolbar is translucent.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isTranslucent: Bool { get set }
```

## Discussion

When the toolbar is translucent, configure the edgesForExtendedLayout and extendedLayoutIncludesOpaqueBars properties of your view controller to display your content underneath the toolbar.

If the toolbar doesn’t have a custom background image, or if any pixel of the background image has an alpha value of less than `1.0`, the default value of this property is true. If the background image is completely opaque, the default value of this property is false. If you set this property to true and the custom background image is completely opaque, UIKit applies a system-defined opacity of less than `1.0` to the image. If you set this property to false and the background image isn’t opaque, UIKit adds an opaque backdrop.

## See Also

### Customizing appearance

var standardAppearance: UIToolbarAppearance

The appearance settings to use for a standard-height toolbar.

var compactAppearance: UIToolbarAppearance?

The appearance settings to use for a compact-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var compactScrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

Legacy customizations

Customize appearance information directly on the toolbar object.

