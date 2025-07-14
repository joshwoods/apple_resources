

- Media Player
- MPVolumeView
-  isWirelessRouteActive Deprecated

Instance Property

# isWirelessRouteActive

A Boolean value that indicates whether the wireless route is active.

iOS 7.0–13.0DeprecatediPadOS 7.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSDeprecated

``` source
@MainActor
var isWirelessRouteActive: Bool { get }
```

Deprecated

Use AVPlayer.externalPlaybackActive instead.

## Discussion

When set to true, the wireless route is active.

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

func routeButtonImage(for: UIControl.State) -> UIImage?

Returns the button image associated with the specified control state.

Deprecated

func routeButtonRect(forBounds: CGRect) -> CGRect

Returns the drawing rectangle for the route button.

Deprecated

func setRouteButtonImage(UIImage?, for: UIControl.State)

Assigns a button image to the specified control states.

Deprecated

