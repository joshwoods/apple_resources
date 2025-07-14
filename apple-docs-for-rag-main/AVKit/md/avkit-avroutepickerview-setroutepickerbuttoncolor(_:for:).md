

- AVKit
- AVRoutePickerView
-  setRoutePickerButtonColor(\_:for:) 

Instance Method

# setRoutePickerButtonColor(\_:for:)

Sets the route picker button color for the specified state.

macOS 10.15+

``` source
@MainActor
func setRoutePickerButtonColor(
    _ color: NSColor?,
    for state: AVRoutePickerView.ButtonState
)
```

## Parameters 

`color`  

The route picker button color to set.

`state`  

The button state.

## See Also

### Configuring the route picker view

var activeTintColor: UIColor!

The view’s tint color when AirPlay is active.

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

enum ButtonState

Constants that describe the available button states.

