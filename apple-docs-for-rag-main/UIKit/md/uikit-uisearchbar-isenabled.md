

- UIKit
- UISearchBar
-  isEnabled 

Instance Property

# isEnabled

A Boolean value indicating whether the search bar is in the enabled state.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+tvOS 16.4+visionOS 1.0+

``` source
@MainActor
var isEnabled: Bool { get set }
```

## Discussion

Set the value of this property to `true` to enable the search bar or `false` to disable it. An enabled search bar responds to user interactions; a disabled search bar ignores touch events and takes on a disabled appearance.

If the search bar is associated with a UINavigationItem with UINavigationItem.SearchBarPlacement.inline, then the minimized (icon-only) UISearchBar won’t grow to the text field while isEnabled is `false`.

The default value of this property is `true` for a newly created search bar. You can set the search bar’s initial enabled state in your storyboard file.

## See Also

### Configuring the search bar

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

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

