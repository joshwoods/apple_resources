

- UIKit
- UISearchBar
-  tintColor 

Instance Property

# tintColor

The tint color to apply to key elements in the search bar.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var tintColor: UIColor! { get set }
```

## Discussion

In iOS v7.0, all subclasses of UIView derive their behavior for tintColor from the base class. See the discussion of tintColor at the UIView level for more information.

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

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

