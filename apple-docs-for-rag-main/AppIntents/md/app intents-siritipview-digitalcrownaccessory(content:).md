

- App Intents
- SiriTipView
-  digitalCrownAccessory(content:) 

Instance Method

# digitalCrownAccessory(content:)

Places an accessory View next to the Digital Crown on Apple Watch.

AppIntentsSwiftUIwatchOS 9.0+

``` source
nonisolated
func digitalCrownAccessory(@ViewBuilder content: @escaping () -> Content) -> some View where Content : View
```

## Parameters 

`content`  

The view to be used as a Digital Crown Accessory.

## Discussion

Use this method to place a custom `View` next to the Digital Crown on Apple Watch. Use `View/digitalCrownAccessory(_:)` to specify the visibility of your custom view.

```
struct ZoomingMapView: View {
    // Width of the map displayed on screen in miles
    @State private var zoomLevel: Int = 1.0

    var body: some View {
        CustomMap(width: .miles(zoomLevel))
            .focusable()
            .digitalCrownRotation(value: $zoomLevel)
            .digitalCrownAccessory {
                Text("\(zoomLevel, specifier: "%.2f")MI")
                .background {
                    RoundedRectangle(cornerRadius: 5)
                        .fill(Color.gray)
                }
            }
    }
}
```

