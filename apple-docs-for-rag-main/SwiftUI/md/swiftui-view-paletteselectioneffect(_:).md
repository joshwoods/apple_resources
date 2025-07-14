

- SwiftUI
- View
-  paletteSelectionEffect(\_:) 

Instance Method

# paletteSelectionEffect(\_:)

Specifies the selection effect to apply to a palette item.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func paletteSelectionEffect(_ effect: PaletteSelectionEffect) -> some View
```

## Parameters 

`effect`  

The type of effect to apply when a palette item is selected.

## Discussion

automatic applies the system’s default appearance when selected. When using un-tinted SF Symbols or template images, the current tint color is applied to the selected items’ image. If the provided SF Symbols have custom tints, a stroke is drawn around selected items.

If you wish to provide a specific image (or SF Symbol) to indicate selection, use custom to forgo the system’s default selection appearance allowing the provided image to solely indicate selection instead.

The following example creates a palette picker that disables the system selection behavior:

```
Menu {
    Picker("Palettes", selection: $selection) {
        ForEach(palettes) { palette in
            Label(palette.title, image: selection == palette ?
                  "selected-palette" : "palette")
            .tint(palette.tint)
            .tag(palette)
        }
    }
    .pickerStyle(.palette)
    .paletteSelectionEffect(.custom)
} label: {
    ...
}
```

If a specific SF Symbol variant is preferable instead, use symbolVariant(_:).

```
Menu {
    ControlGroup {
        ForEach(ColorTags.allCases) { colorTag in
            Toggle(isOn: $selectedColorTags[colorTag]) {
                Label(colorTag.name, systemImage: "circle")
            }
            .tint(colorTag.color)
        }
    }
    .controlGroupStyle(.palette)
    .paletteSelectionEffect(.symbolVariant(.fill))
}
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

var defaultWheelPickerItemHeight: CGFloat

The default height of an item in a wheel-style picker, such as a date picker.

struct PaletteSelectionEffect

The selection effect to apply to a palette item.

