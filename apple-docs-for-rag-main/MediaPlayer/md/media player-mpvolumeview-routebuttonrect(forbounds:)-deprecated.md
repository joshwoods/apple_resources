

- Media Player
- MPVolumeView
-  routeButtonRect(forBounds:) Deprecated

Instance Method

# routeButtonRect(forBounds:)

Returns the drawing rectangle for the route button.

iOS 6.0–13.0DeprecatediPadOS 6.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
func routeButtonRect(forBounds bounds: CGRect) -> CGRect
```

Deprecated

See AVRoutePickerView for possible replacements.

## Parameters 

`bounds`  

The bounding rectangle of the receiver.

## Return Value

The computed drawing rectangle for the route button.

## Discussion

Use this method to retrieve the bounding rectangle for the route button.

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

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

