

- UIKit
- UISearchBar
-  barTintColor 

Instance Property

# barTintColor

The tint color to apply to the search bar background.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var barTintColor: UIColor? { get set }
```

## Discussion

This color is made translucent by default unless you set the isTranslucent property to false.

## See Also

### Configuring the search bar

var isEnabled: Bool

A Boolean value indicating whether the search bar is in the enabled state.

var searchBarStyle: UISearchBar.Style

A search bar style that specifies the search bar’s appearance.

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

