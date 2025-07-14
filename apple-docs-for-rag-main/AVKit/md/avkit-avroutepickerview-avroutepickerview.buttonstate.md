

- AVKit
- AVRoutePickerView
-  AVRoutePickerView.ButtonState 

Enumeration

# AVRoutePickerView.ButtonState

Constants that describe the available button states.

macOS 10.15+

``` source
enum ButtonState
```

## Topics

### Button States

case normal

The normal, or default, button state.

case normalHighlighted

The highlighted button state when a mouse-down event occurs inside the button.

case active

The button state when AirPlay is active.

case activeHighlighted

The highlighted button state when AirPlay is active.

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

enum AVRoutePickerViewButtonStyle

Constants that define the button styles a route picker view supports.

func routePickerButtonColor(for: AVRoutePickerView.ButtonState) -> NSColor

Returns the color of the picker button for the specified state.

func setRoutePickerButtonColor(NSColor?, for: AVRoutePickerView.ButtonState)

Sets the route picker button color for the specified state.

