

- UIKit
- UISearchBar
-  UISearchBar.Style 

Enumeration

# UISearchBar.Style

Specifies whether the search bar has a background.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
enum Style
```

## Topics

### Constants

case `default`

The search bar has the default style.

case prominent

The search bar has a translucent background, and the search field is opaque.

case minimal

The search bar has no background, and the search field is translucent.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring the search bar

var isEnabled: Bool

A Boolean value indicating whether the search bar is in the enabled state.

var barTintColor: UIColor?

The tint color to apply to the search bar background.

var searchBarStyle: UISearchBar.Style

A search bar style that specifies the search bar’s appearance.

var tintColor: UIColor!

The tint color to apply to key elements in the search bar.

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

enum UIBarStyle

Defines the stylistic appearance of different types of views.

