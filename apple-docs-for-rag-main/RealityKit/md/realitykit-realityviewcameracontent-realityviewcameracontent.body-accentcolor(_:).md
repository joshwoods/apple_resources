

- RealityKit
- RealityViewCameraContent
- RealityViewCameraContent.Body
-  accentColor(\_:) 

Instance Method

# accentColor(\_:)

Sets the accent color for this view and the views it contains.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac CatalystmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func accentColor(_ accentColor: Color?) -> some View
```

## Parameters 

`accentColor`  

The color to use as an accent color. Set the value to `nil` to use the inherited accent color.

## Discussion

Use `accentColor(_:)` when you want to apply a broad theme color to your app’s user interface. Some styles of controls use the accent color as a default tint color.

Note

In macOS, SwiftUI applies customization of the accent color only if the user chooses Multicolor under General \> Accent color in System Preferences.

In the example below, the outer `VStack` contains two child views. The first is a button with the default accent color. The second is a `VStack` that contains a button and a slider, both of which adopt the purple accent color of their containing view. Note that the `Text` element used as a label alongside the `Slider` retains its default color.

```
VStack(spacing: 20) {
    Button(action: {}) {
        Text("Regular Button")
    }
    VStack {
        Button(action: {}) {
            Text("Accented Button")
        }
        HStack {
            Text("Accented Slider")
            Slider(value: $sliderValue, in: -100...100, step: 0.1)
        }
    }
    .accentColor(.purple)
}
```

