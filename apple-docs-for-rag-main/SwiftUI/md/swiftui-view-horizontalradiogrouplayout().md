

- SwiftUI
- View
-  horizontalRadioGroupLayout() 

Instance Method

# horizontalRadioGroupLayout()

Sets the style for radio group style pickers within this view to be horizontally positioned with the radio buttons inside the layout.

macOS 10.15+

``` source
nonisolated
func horizontalRadioGroupLayout() -> some View
```

## Discussion

Use `horizontalRadioGroupLayout()` to configure the visual layout of radio buttons in a Picker so that the radio buttons are arranged horizontally in the view.

The example below shows two Picker controls configured as radio button groups; the first group shows the default vertical layout; the second group shows the effect of `horizontalRadioGroupLayout()` which renders the radio buttons horizontally.

```
struct HorizontalRadioGroupLayout: View {
    @State private var selected = 1
    var body: some View {
        VStack(spacing: 20) {
            Picker(selection: $selected, label: Text("Favorite Color")) {
                Text("Red").tag(1)
                Text("Green").tag(2)
                Text("Blue").tag(3)
                Text("Other").tag(4)
            }
            .pickerStyle(.radioGroup)

            Picker(selection: $selected, label: Text("Favorite Color")) {
                Text("Red").tag(1)
                Text("Green").tag(2)
                Text("Blue").tag(3)
                Text("Other").tag(4)
            }
            .pickerStyle(.radioGroup)
            .horizontalRadioGroupLayout()
        }
        .padding(20)
        .border(Color.gray)
    }
}
```

## See Also

### Choosing from a set of options

struct Picker

A control for selecting from a set of mutually exclusive values.

func pickerStyle&lt;S>(S) -> some View

Sets the style for pickers within this view.

func defaultWheelPickerItemHeight(CGFloat) -> some View

Sets the default wheel-style picker item height.

var defaultWheelPickerItemHeight: CGFloat

The default height of an item in a wheel-style picker, such as a date picker.

func paletteSelectionEffect(PaletteSelectionEffect) -> some View

Specifies the selection effect to apply to a palette item.

struct PaletteSelectionEffect

The selection effect to apply to a palette item.

