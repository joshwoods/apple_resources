

- UIKit
- UISearchBar
-  isTranslucent 

Instance Property

# isTranslucent

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var isTranslucent: Bool { get set }
```

## Discussion

The default value is true. If the search bar has a custom background image, the default is true if any pixel of the image has an alpha value of less than `1.0`, and false otherwise.

If you set this property to true on a search bar with an opaque custom background image, the search bar will apply a system opacity less than `1.0` to the image.

If you set this property to false on a search bar with a translucent custom background image, the search bar provides an opaque background for the image using black if the search bar has UIBarStyle.black style, white if the search bar has UIBarStyle.default, or the search bar’s barTintColor if a custom value is defined.

## See Also

### Configuring the search bar

var isEnabled: Bool

A Boolean value indicating whether the search bar is in the enabled state.

var barTintColor: UIColor?

The tint color to apply to the search bar background.

var searchBarStyle: UISearchBar.Style

A search bar style that specifies the search bar’s appearance.

enum Style

Specifies whether the search bar has a background.

var tintColor: UIColor!

The tint color to apply to key elements in the search bar.

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

