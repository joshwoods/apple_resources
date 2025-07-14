

- UIKit
- UISearchBar
-  barStyle 

Instance Property

# barStyle

A bar style that specifies the search bar’s appearance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var barStyle: UIBarStyle { get set }
```

## Discussion

This property can be used together with searchBarStyle.

See UIBarStyle for possible values. The default value is UIBarStyle.default.

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

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

enum UIBarStyle

Defines the stylistic appearance of different types of views.

