

- SwiftUI
- EnvironmentValues
-  defaultWheelPickerItemHeight 

Instance Property

# defaultWheelPickerItemHeight

The default height of an item in a wheel-style picker, such as a date picker.

watchOS 6.0+

``` source
var defaultWheelPickerItemHeight: CGFloat { get set }
```

## See Also

### Choosing from a set of options

struct Picker

A control for selecting from a set of mutually exclusive values.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func horizontalRadioGroupLayout() -> some View

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

struct PaletteSelectionEffect

The selection effect to apply to a palette item.

