

- UIKit
- UISearchBar
-  backgroundImage(for:barMetrics:) 

Instance Method

# backgroundImage(for:barMetrics:)

Returns the image used for the background in a given position and with given metrics.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundImage(
    for barPosition: UIBarPosition,
    barMetrics: UIBarMetrics
) -> UIImage?
```

## Parameters 

`barPosition`  

A bar position constant.

`barMetrics`  

A bar metrics constant.

## Return Value

The image used for the search bar background in the position specified by `barPosition` and with the metrics specified by `barMetrics`.

## Discussion

The default value is `nil`.

## See Also

### Customizing the search bar appearance

var backgroundImage: UIImage?

The background image for the search bar.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the image to use for the background in a given position and with given metrics.

func image(for: UISearchBar.Icon, state: UIControl.State) -> UIImage?

Returns the image for a given search bar icon type and control state.

func setImage(UIImage?, for: UISearchBar.Icon, state: UIControl.State)

Sets the image for a given search bar icon type and control state.

func positionAdjustment(for: UISearchBar.Icon) -> UIOffset

Returns the position adjustment for a given icon.

func setPositionAdjustment(UIOffset, for: UISearchBar.Icon)

Returns the position adjustment for a given icon.

var inputAccessoryView: UIView?

A custom input accessory view for the keyboard of the search bar.

func searchFieldBackgroundImage(for: UIControl.State) -> UIImage?

Returns the search text field image for a given state.

func setSearchFieldBackgroundImage(UIImage?, for: UIControl.State)

Sets the search text field image for a given state.

var searchFieldBackgroundPositionAdjustment: UIOffset

The offset of the search text field background in the search bar.

var searchTextPositionAdjustment: UIOffset

The offset of the text within the search text field background.

