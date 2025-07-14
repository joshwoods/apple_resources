

- UIKit
- UITabBar
-  leadingAccessoryView 

Instance Property

# leadingAccessoryView

The view at the leading edge of a tab bar on tvOS.

tvOS 13.0+

``` source
@MainActor
var leadingAccessoryView: UIView { get }
```

## Discussion

Use this property to integrate a custom view at the leading edge of your tab bar interface. Use this view to display a custom logo or give access to custom accessories in your app.

## See Also

### Customizing tab bar appearance

var standardAppearance: UITabBarAppearance

The appearance settings for a standard-height tab bar.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var trailingAccessoryView: UIView

The view at the trailing edge of a tab bar on tvOS.

var isTranslucent: Bool

A Boolean value that indicates whether the tab bar is translucent.

Legacy customizations

Customize appearance information directly on the tab bar object.

