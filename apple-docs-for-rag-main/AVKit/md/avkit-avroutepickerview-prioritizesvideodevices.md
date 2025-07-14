

- AVKit
- AVRoutePickerView
-  prioritizesVideoDevices 

Instance Property

# prioritizesVideoDevices

A Boolean value that indicates whether the route picker sorts video output devices to the top of the list.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+

``` source
@MainActor
var prioritizesVideoDevices: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Configuring the route picker view

var activeTintColor: UIColor!

The view’s tint color when AirPlay is active.

var isRoutePickerButtonBordered: Bool

A Boolean value that indicates whether the route picker button has a border.

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

