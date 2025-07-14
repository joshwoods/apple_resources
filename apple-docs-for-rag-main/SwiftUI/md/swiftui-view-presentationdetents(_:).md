

- SwiftUI
- View
-  presentationDetents(\_:) 

Instance Method

# presentationDetents(\_:)

Sets the available detents for the enclosing sheet.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func presentationDetents(_ detents: Set) -> some View
```

## Parameters 

`detents`  

A set of supported detents for the sheet. If you provide more that one detent, people can drag the sheet to resize it.

## Discussion

By default, sheets support the large detent.

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

## See Also

### Configuring a sheet’s height

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationContentInteraction(PresentationContentInteraction) -> some View

Configures the behavior of swipe gestures on a presentation.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

struct PresentationDetent

A type that represents a height where a sheet naturally rests.

protocol CustomPresentationDetent

The definition of a custom detent with a calculated height.

struct PresentationContentInteraction

A behavior that you can use to influence how a presentation responds to swipe gestures.

