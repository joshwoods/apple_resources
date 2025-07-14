

- Media Player
- MPVolumeView
-  showsRouteButton Deprecated

Instance Property

# showsRouteButton

A Boolean value that indicates whether the route button is visible in the volume view.

iOS 4.2–13.0DeprecatediPadOS 4.2–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var showsRouteButton: Bool { get set }
```

Deprecated

Use AVRoutePickerView instead.

## Discussion

The route button is visible by default when there’s more than one audio output route available. To hide the route button, set this property’s value to false.

## See Also

### Deprecated

var volumeWarningSliderImage: UIImage?

The image used to designate the European Union volume limit.

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

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

