

- UIKit
- UINavigationBar
-  compactScrollEdgeAppearance 

Instance Property

# compactScrollEdgeAppearance

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var compactScrollEdgeAppearance: UINavigationBarAppearance? { get set }
```

## Discussion

When a navigation controller contains a navigation bar and a scroll view, part of the scroll view’s content appears underneath the navigation bar. If the edge of the scrolled content reaches that bar, UIKit applies the appearance settings in this property.

This property applies to compact-height navigation bars. If the value of this property is `nil`, UIKit uses the value of the scrollEdgeAppearance of the navigation bar. If no navigation controller manages your navigation bar, UIKit ignores this property and uses the compactAppearance of the navigation bar.

You can customize the appearance of the navigation bar based on the top navigation item with the compactScrollEdgeAppearance property of UINavigationItem.

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

var isTranslucent: Bool

A Boolean value that indicates whether the navigation bar is translucent.

Legacy customizations

Customize appearance information directly on the navigation bar object.

