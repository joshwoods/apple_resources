

- Media Player
- MPVolumeView
-  routeButtonImage(for:) Deprecated

Instance Method

# routeButtonImage(for:)

Returns the button image associated with the specified control state.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func routeButtonImage(for state: UIControl.State) -> UIImage?
```

Deprecated

See AVRoutePickerView for possible replacements.

## Parameters 

`state`  

The control state whose thumb image you want. You should specify only one control state value for this parameter.

## Return Value

The button image associated with the specified state, or nil if an appropriate image could not be retrieved. This method might return nil if you specify multiple control states in the state parameter.

## Discussion

Use this method to retrieve the corresponding button image for a specific state.

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

func routeButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the route button.

Deprecated

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

