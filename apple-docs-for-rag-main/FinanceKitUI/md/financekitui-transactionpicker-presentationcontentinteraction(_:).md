

- FinanceKitUI
- TransactionPicker
-  presentationContentInteraction(\_:) 

Instance Method

# presentationContentInteraction(\_:)

Configures the behavior of swipe gestures on a presentation.

FinanceKitUISwiftUIiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+watchOS 9.4+

``` source
nonisolated
func presentationContentInteraction(_ behavior: PresentationContentInteraction) -> some View
```

## Parameters 

`behavior`  

The requested behavior.

## Discussion

By default, when a person swipes up on a scroll view in a resizable presentation, the presentation grows to the next detent. A scroll view embedded in the presentation only scrolls after the presentation reaches its largest size. Use this modifier to control which action takes precedence.

For example, you can request that swipe gestures scroll content first, resizing the sheet only after hitting the end of the scroll view, by passing the `PresentationContentInteraction/scrolls` value to this modifier:

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

