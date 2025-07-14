

- SwiftUI
- View
-  presentationBackground(\_:) 

Instance Method

# presentationBackground(\_:)

Sets the presentation background of the enclosing sheet using a shape style.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
nonisolated
func presentationBackground(_ style: S) -> some View where S : ShapeStyle
```

## Parameters 

`style`  

The shape style to use as the presentation background.

## Discussion

The following example uses the thick material as the sheet background:

```
struct ContentView: View {
    @State private var showSettings = false

    var body: some View {
        Button("View Settings") {
            showSettings = true
        }
        .sheet(isPresented: $showSettings) {
            SettingsView()
                .presentationBackground(.thickMaterial)
        }
    }
}
```

The `presentationBackground(_:)` modifier differs from the background(_:ignoresSafeAreaEdges:) modifier in several key ways. A presentation background:

- Automatically fills the entire presentation.

- Allows views behind the presentation to show through translucent styles.

## See Also

### Styling a sheet and its background

func presentationCornerRadius(CGFloat?) -> some View

Requests that the presentation have a specific corner radius.

func presentationBackground&lt;V>(alignment: Alignment, content: () -> V) -> some View

Sets the presentation background of the enclosing sheet to a custom view.

func presentationBackgroundInteraction(PresentationBackgroundInteraction) -> some View

Controls whether people can interact with the view behind a presentation.

struct PresentationBackgroundInteraction

The kinds of interaction available to views behind a presentation.

