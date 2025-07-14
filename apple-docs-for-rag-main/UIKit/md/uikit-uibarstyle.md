

- UIKit
-  UIBarStyle 

Enumeration

# UIBarStyle

Defines the stylistic appearance of different types of views.

iOSiPadOSMac CatalystvisionOS

``` source
enum UIBarStyle
```

## Topics

### Bar styles

case `default`

The default style normally associated with the given view.

case black

A black background with light content.

static var blackOpaque: UIBarStyle

A deprecated opaque style.

Deprecated

case blackTranslucent

A deprecated translucent style.

Deprecated

### Initializers

init?(rawValue: Int)

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

enum Style

Specifies whether the search bar has a background.

var tintColor: UIColor!

The tint color to apply to key elements in the search bar.

var isTranslucent: Bool

A Boolean value that indicates whether the search bar is translucent (true) or not (false).

var barStyle: UIBarStyle

A bar style that specifies the search bar’s appearance.

