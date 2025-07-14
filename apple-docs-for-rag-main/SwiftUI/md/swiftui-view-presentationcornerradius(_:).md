

- SwiftUI
- View
-  presentationCornerRadius(\_:) 

Instance Method

# presentationCornerRadius(\_:)

Requests that the presentation have a specific corner radius.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

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

## See Also

### Styling a sheet and its background

func presentationBackground&lt;S>(S) -> some View

Sets the presentation background of the enclosing sheet using a shape style.

func presentationBackground&lt;V>(alignment: Alignment, content: () -> V) -> some View

Sets the presentation background of the enclosing sheet to a custom view.

func presentationBackgroundInteraction(PresentationBackgroundInteraction) -> some View

Controls whether people can interact with the view behind a presentation.

struct PresentationBackgroundInteraction

The kinds of interaction available to views behind a presentation.

