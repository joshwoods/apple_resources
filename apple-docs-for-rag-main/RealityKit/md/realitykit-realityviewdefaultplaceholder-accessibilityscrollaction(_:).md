

- RealityKit
- RealityViewDefaultPlaceholder
-  accessibilityScrollAction(\_:) 

Instance Method

# accessibilityScrollAction(\_:)

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+Mac CatalystmacOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func accessibilityScrollAction(_ handler: @escaping (Edge) -> Void) -> ModifiedContent
```

## Discussion

For example, this is how a scroll action to trigger a refresh could be added to a view.

```
var body: some View {
    ScrollView {
        ContentView()
    }
    .accessibilityScrollAction { edge in
        if edge == .top {
            // Refresh content
        }
    }
}
```

