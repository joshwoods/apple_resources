

- Media Player
- MPVolumeView
-  setRouteButtonImage(\_:for:) Deprecated

Instance Method

# setRouteButtonImage(\_:for:)

Assigns a button image to the specified control states.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func setRouteButtonImage(
    _ image: UIImage?,
    for state: UIControl.State
)
```

Deprecated

Use AVRoutePickerView.routePickerButtonStyle instead.

## Parameters 

`image`  

The image to associate with the specified states.

`state`  

The control state with which to associate the image.

## Discussion

Use this to customize the appearance of the route button for various states such as enabled, disabled, and highlighted.

## See Also

### Deprecated

var volumeWarningSliderImage: UIImage?

The image used to designate the European Union volume limit.

Deprecated

var showsRouteButton: Bool

A Boolean value that indicates whether the route button is visible in the volume view.

Deprecated

var areWirelessRoutesAvailable: Bool

A Boolean value indicating wireless routes are available.

Deprecated

var isWirelessRouteActive: Bool

A Boolean value that indicates whether the wireless route is active.

Deprecated

func routeButtonImage(for: UIControl.State) -> UIImage?

Returns the button image associated with the specified control state.

Deprecated

func routeButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the route button.

Deprecated

