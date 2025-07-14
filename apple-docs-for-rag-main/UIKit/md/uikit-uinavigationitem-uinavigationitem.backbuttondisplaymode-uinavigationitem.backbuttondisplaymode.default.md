

- UIKit
- UINavigationItem
- UINavigationItem.BackButtonDisplayMode
-  UINavigationItem.BackButtonDisplayMode.default 

Case

# UINavigationItem.BackButtonDisplayMode.default

The navigation item attempts to display a specific title, a generic title, or no title for the Back button, depending on the space available.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case `default`
```

## Discussion

When you set the backButtonDisplayMode property to this value, the navigation item attempts to display these titles for its Back button in the following order:

- backButtonTitle

- title

- A generic title, such as *Back*

- No title

The navigation item selects the most appropriate title for the Back button according to the available space.

## See Also

### Constants

case generic

The navigation item attempts to display a generic title or no title for the Back button, depending on the space available.

case minimal

The navigation item displays the Back button indicator instead of a title.

