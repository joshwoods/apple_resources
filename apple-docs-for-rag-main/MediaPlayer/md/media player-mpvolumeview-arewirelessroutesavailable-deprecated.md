

- Media Player
- MPVolumeView
-  areWirelessRoutesAvailable Deprecated

Instance Property

# areWirelessRoutesAvailable

A Boolean value indicating wireless routes are available.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var areWirelessRoutesAvailable: Bool { get }
```

Deprecated

Use AVRouteDetector.multipleRoutesDetected instead.

## Discussion

When set to true, a wireless route is available for user selection. Some types of wireless routes are only discovered when the view is present in the window hierarchy.

## See Also

### Deprecated

var volumeWarningSliderImage: UIImage?

The image used to designate the European Union volume limit.

Deprecated

var showsRouteButton: Bool

A Boolean value that indicates whether the route button is visible in the volume view.

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

