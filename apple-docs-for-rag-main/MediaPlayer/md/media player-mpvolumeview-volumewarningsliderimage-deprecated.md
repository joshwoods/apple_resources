

- Media Player
- MPVolumeView
-  volumeWarningSliderImage Deprecated

Instance Property

# volumeWarningSliderImage

The image used to designate the European Union volume limit.

iOS 7.0–17.0DeprecatediPadOS 7.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecated

``` source
@MainActor
var volumeWarningSliderImage: UIImage? { get set }
```

Deprecated

This is no longer supported

## Discussion

The system displays the image contained by this property on top of the maximumVolumeSliderImage(for:). The image must be visually distinct from the `maximumVolumeSliderImage` and use a color similar to the default in order to convey a sense of warning to the user.

For testing purposes, set the EU Volume Limit setting in the Developer menu of the Settings app to always enable the volume limit.

## See Also

### Deprecated

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

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

