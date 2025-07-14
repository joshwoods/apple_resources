

- SwiftUI
- View
-  presentationCompactAdaptation(\_:) 

Instance Method

# presentationCompactAdaptation(\_:)

Specifies how to adapt a presentation to compact size classes.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
nonisolated
func presentationCompactAdaptation(_ adaptation: PresentationAdaptation) -> some View
```

## Parameters 

`adaptation`  

The adaptation to use in either a horizontally or vertically compact size class.

## Discussion

Some presentations adapt their appearance depending on the context. For example, a sheet presentation over a vertically-compact view uses a full-screen-cover appearance by default. Use this modifier to indicate a custom adaptation preference. For example, the following code uses a presentation adaptation value of none to request that the system not adapt the sheet in compact size classes:

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
                .presentationCompactAdaptation(.none)
        }
    }
}
```

If you want to specify different adaptations for each dimension, use the presentationCompactAdaptation(horizontal:vertical:) method instead.

## See Also

### Adapting a presentation size

func presentationCompactAdaptation(horizontal: PresentationAdaptation, vertical: PresentationAdaptation) -> some View

Specifies how to adapt a presentation to horizontally and vertically compact size classes.

struct PresentationAdaptation

Strategies for adapting a presentation to a different size class.

func presentationSizing(some PresentationSizing) -> some View

Sets the sizing of the containing presentation.

protocol PresentationSizing

A type that defines the size of the presentation content and how the presentation size adjusts to its content’s size changing.

struct PresentationSizingRoot

A proxy to a view provided to the presentation with a defined presentation size.

struct PresentationSizingContext

Contextual information about a presentation.

