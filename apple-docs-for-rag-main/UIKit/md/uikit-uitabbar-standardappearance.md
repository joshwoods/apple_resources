

- UIKit
- UITabBar
-  standardAppearance 

Instance Property

# standardAppearance

The appearance settings for a standard-height tab bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var standardAppearance: UITabBarAppearance { get set }
```

## Discussion

The default value of this property is an appearance object containing the system’s default appearance settings.

## See Also

### Customizing tab bar appearance

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var leadingAccessoryView: UIView

The view at the leading edge of a tab bar on tvOS.

var trailingAccessoryView: UIView

The view at the trailing edge of a tab bar on tvOS.

var isTranslucent: Bool

A Boolean value that indicates whether the tab bar is translucent.

Legacy customizations

Customize appearance information directly on the tab bar object.

