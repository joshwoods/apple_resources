

- UIKit
- UISearchBar
-  searchBarStyle 

Instance Property

# searchBarStyle

A search bar style that specifies the search bar’s appearance.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var searchBarStyle: UISearchBar.Style { get set }
```

## Discussion

This property can be used together with barStyle. The style UISearchBar.Style.minimal provides no default background color or image but will display one if customized as such.

Custom background and search field images take precedence over this property.

See UISearchBar.Style for possible values. The default value is UISearchBar.Style.default.

## See Also

### Configuring the search bar

var isEnabled: Bool

A Boolean value indicating whether the search bar is in the enabled state.

var barTintColor: UIColor?

The tint color to apply to the search bar background.

enum Style

Specifies whether the search bar has a background.

var tintColor: UIColor!

The tint color to apply to key elements in the search bar.

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

