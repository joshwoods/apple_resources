

- RealityKit
- RealityViewDefaultPlaceholder
-  presentationCornerRadius(\_:) 

Instance Method

# presentationCornerRadius(\_:)

Requests that the presentation have a specific corner radius.

RealityKitSwiftUIiOS 16.4+iPadOS 16.4+Mac CatalystmacOS 13.3+tvOS 16.4+visionOSwatchOS 9.4+

``` source
nonisolated
func presentationCornerRadius(_ cornerRadius: CGFloat?) -> some View
```

## Parameters 

`cornerRadius`  

The corner radius, or `nil` to use the system default.

## Discussion

Use this modifier to change the corner radius of a presentation.

```
struct ContentView: View {
    @State private var showSettings = false

    var body: some View {
        Button("View Settings") {
            showSettings = true
        }
        .sheet(isPresented: $showSettings) {
            SettingsView()
                .presentationDetents([.medium, .large])
                .presentationCornerRadius(21)
        }
    }
}
```

