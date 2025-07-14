

- MusicKit
- ArtworkImage
-  presentationDetents(\_:) 

Instance Method

# presentationDetents(\_:)

Sets the available detents for the enclosing sheet.

MusicKitSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func presentationDetents(_ detents: Set) -> some View
```

## Parameters 

`detents`  

A set of supported detents for the sheet. If you provide more that one detent, people can drag the sheet to resize it.

## Discussion

By default, sheets support the `PresentationDetent/large` detent.

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
        }
    }
}
```

