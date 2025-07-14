

- RealityKit
- ObjectCapturePointCloudView
-  presentationCompactAdaptation(horizontal:vertical:) 

Instance Method

# presentationCompactAdaptation(horizontal:vertical:)

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

RealityKitSwiftUIiOS 16.4+iPadOS 16.4+macOS 13.3+tvOS 16.4+watchOS 9.4+

``` source
nonisolated
func presentationCompactAdaptation(
    horizontal horizontalAdaptation: PresentationAdaptation,
    vertical verticalAdaptation: PresentationAdaptation
) -> some View
```

## Parameters 

`horizontalAdaptation`  

The adaptation to use in a horizontally compact size class.

`verticalAdaptation`  

The adaptation to use in a vertically compact size class. In a size class that is both horizontally and vertically compact, SwiftUI uses the `verticalAdaptation` value.

## Discussion

Some presentations adapt their appearance depending on the context. For example, a popover presentation over a horizontally-compact view uses a sheet appearance by default. Use this modifier to indicate a custom adaptation preference.

```
struct ContentView: View {
    @State private var showInfo = false

    var body: some View {
        Button("View Info") {
            showInfo = true
        }
        .popover(isPresented: $showInfo) {
            InfoView()
                .presentationCompactAdaptation(
                    horizontal: .popover,
                    vertical: .sheet)
        }
    }
}
```

If you want to specify the same adaptation for both dimensions, use the `View/presentationCompactAdaptation(_:)` method instead.

