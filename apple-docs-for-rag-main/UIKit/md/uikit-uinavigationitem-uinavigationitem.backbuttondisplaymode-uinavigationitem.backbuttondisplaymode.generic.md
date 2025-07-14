

- UIKit
- UINavigationItem
- UINavigationItem.BackButtonDisplayMode
-  UINavigationItem.BackButtonDisplayMode.generic 

Case

# UINavigationItem.BackButtonDisplayMode.generic

The navigation item attempts to display a generic title or no title for the Back button, depending on the space available.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
case generic
```

## Discussion

When you set the backButtonDisplayMode property to this value, the navigation item attempts to display these titles for its Back button in the following order:

- A generic title, such as *Back*

- No title

The navigation item selects the most appropriate title for the Back button according to the available space. This display mode ignores the values of the title and backButtonTitle properties.

## See Also

### Constants

case `default`

The navigation item attempts to display a specific title, a generic title, or no title for the Back button, depending on the space available.

case minimal

The navigation item displays the Back button indicator instead of a title.

