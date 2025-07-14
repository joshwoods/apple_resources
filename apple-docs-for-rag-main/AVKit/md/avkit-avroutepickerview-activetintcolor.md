

- AVKit
- AVRoutePickerView
-  activeTintColor 

Instance Property

# activeTintColor

The view’s tint color when AirPlay is active.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 11.0+

``` source
@MainActor
var activeTintColor: UIColor! { get set }
```

## See Also

### Configuring the route picker view

var isRoutePickerButtonBordered: Bool

A Boolean value that indicates whether the route picker button has a border.

var prioritizesVideoDevices: Bool

A Boolean value that indicates whether the route picker sorts video output devices to the top of the list.

var routePickerButtonStyle: AVRoutePickerViewButtonStyle

The button style for the route picker.

enum AVRoutePickerViewButtonStyle

Constants that define the button styles a route picker view supports.

func routePickerButtonColor(for: AVRoutePickerView.ButtonState) -> NSColor

Returns the color of the picker button for the specified state.

func setRoutePickerButtonColor(NSColor?, for: AVRoutePickerView.ButtonState)

Sets the route picker button color for the specified state.

enum ButtonState

Constants that describe the available button states.

