

- AVKit
- AVRoutePickerView
-  routePickerButtonColor(for:) 

Instance Method

# routePickerButtonColor(for:)

Returns the color of the picker button for the specified state.

macOS 10.15+

``` source
@MainActor
func routePickerButtonColor(for state: AVRoutePickerView.ButtonState) -> NSColor
```

## Parameters 

`state`  

The button state.

## Return Value

A color value for the specified state.

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

func setRoutePickerButtonColor(NSColor?, for: AVRoutePickerView.ButtonState)

Sets the route picker button color for the specified state.

enum ButtonState

Constants that describe the available button states.

