

- AVKit
-  AVRoutePickerViewButtonStyle 

Enumeration

# AVRoutePickerViewButtonStyle

Constants that define the button styles a route picker view supports.

tvOS 11.0+

``` source
enum AVRoutePickerViewButtonStyle
```

## Topics

### Button Styles

case custom

A custom button style.

case plain

A plain button style.

case system

A system-defined button style.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func routePickerButtonColor(for: AVRoutePickerView.ButtonState) -> NSColor

Returns the color of the picker button for the specified state.

func setRoutePickerButtonColor(NSColor?, for: AVRoutePickerView.ButtonState)

Sets the route picker button color for the specified state.

enum ButtonState

Constants that describe the available button states.

