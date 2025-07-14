

- UIKit
- UINavigationBar
-  compactAppearance 

Instance Property

# compactAppearance

The appearance settings for a compact-height navigation bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var compactAppearance: UINavigationBarAppearance? { get set }
```

## Discussion

If the value of this property is `nil`, UIKit uses the standardAppearance of the item stored in the topItem property. You can customize the compact appearance for specific navigation items with the compactAppearance property of UINavigationItem.

## See Also

### Customizing the bar’s appearance

var prefersLargeTitles: Bool

A Boolean value that indicates whether the title displays in a large format.

var standardAppearance: UINavigationBarAppearance

The appearance settings for a standard-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for the navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var isTranslucent: Bool

A Boolean value that indicates whether the navigation bar is translucent.

Legacy customizations

Customize appearance information directly on the navigation bar object.

