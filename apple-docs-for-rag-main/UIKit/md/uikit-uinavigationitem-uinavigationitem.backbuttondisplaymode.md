

- UIKit
- UINavigationItem
-  UINavigationItem.BackButtonDisplayMode 

Enumeration

# UINavigationItem.BackButtonDisplayMode

Constants that describe the display modes of the Back button.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum BackButtonDisplayMode
```

## Topics

### Constants

case `default`

The navigation item attempts to display a specific title, a generic title, or no title for the Back button, depending on the space available.

case generic

The navigation item attempts to display a generic title or no title for the Back button, depending on the space available.

case minimal

The navigation item displays the Back button indicator instead of a title.

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

### Configuring the Back button

var backBarButtonItem: UIBarButtonItem?

The bar button item for adding a Back button to the navigation bar.

var backButtonTitle: String?

The custom title of the Back button.

var backButtonDisplayMode: UINavigationItem.BackButtonDisplayMode

The display mode of the Back button.

var hidesBackButton: Bool

A Boolean value that determines whether the navigation item hides the Back button.

func setHidesBackButton(Bool, animated: Bool)

Hides or shows the Back button, optionally animating the transition.

var backAction: UIAction?

The back action for the navigation bar.

