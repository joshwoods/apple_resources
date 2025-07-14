

- RealityKit
- Model3D
-  accessibilityAction(action:label:) 

Instance Method

# accessibilityAction(action:label:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

RealityKitSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
nonisolated
func accessibilityAction(
    action: @escaping () -> Void,
    @ViewBuilder label: () -> Label
) -> some View where Label : View
```

## Discussion

For example, this is how a custom action to compose a new email could be added to a view.

```
var body: some View {
    ContentView()
        .accessibilityAction {
            // Handle action
        } label: {
            Label("New Message", systemImage: "plus")
        }
}
```

