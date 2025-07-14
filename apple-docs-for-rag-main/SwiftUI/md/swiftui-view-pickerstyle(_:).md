

- SwiftUI
- View
-  pickerStyle(\_:) 

Instance Method

# pickerStyle(\_:)

Sets the style for pickers within this view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func pickerStyle(_ style: S) -> some View where S : PickerStyle
```

## See Also

### Choosing from a set of options

struct Picker

A control for selecting from a set of mutually exclusive values.

func horizontalRadioGroupLayout() -> some View

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

var defaultWheelPickerItemHeight: CGFloat

The default height of an item in a wheel-style picker, such as a date picker.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

struct PaletteSelectionEffect

The selection effect to apply to a palette item.

