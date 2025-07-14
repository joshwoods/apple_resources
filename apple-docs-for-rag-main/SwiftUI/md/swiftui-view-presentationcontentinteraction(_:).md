

- SwiftUI
- View
-  presentationContentInteraction(\_:) 

Instance Method

# presentationContentInteraction(\_:)

Configures the behavior of swipe gestures on a presentation.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
nonisolated
func presentationContentInteraction(_ behavior: PresentationContentInteraction) -> some View
```

## Parameters 

`behavior`  

The requested behavior.

## Discussion

By default, when a person swipes up on a scroll view in a resizable presentation, the presentation grows to the next detent. A scroll view embedded in the presentation only scrolls after the presentation reaches its largest size. Use this modifier to control which action takes precedence.

For example, you can request that swipe gestures scroll content first, resizing the sheet only after hitting the end of the scroll view, by passing the scrolls value to this modifier:

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
                .presentationContentInteraction(.scrolls)
        }
    }
}
```

People can always resize your presentation using the drag indicator.

## See Also

### Configuring a sheet’s height

func presentationDetents(Set&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet.

func presentationDetents(Set&lt;PresentationDetent>, selection: Binding&lt;PresentationDetent>) -> some View

Sets the available detents for the enclosing sheet, giving you programmatic control of the currently selected detent.

func presentationDragIndicator(Visibility) -> some View

Sets the visibility of the drag indicator on top of a sheet.

struct PresentationDetent

A type that represents a height where a sheet naturally rests.

protocol CustomPresentationDetent

The definition of a custom detent with a calculated height.

struct PresentationContentInteraction

A behavior that you can use to influence how a presentation responds to swipe gestures.

