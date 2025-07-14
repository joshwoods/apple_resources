

- RealityKit
- ResolvedModel3D
-  accessibilityAction(named:\_:) 

Instance Method

# accessibilityAction(named:\_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func accessibilityAction(
    named name: Text,
    _ handler: @escaping () -> Void
) -> ModifiedContent
```

## Discussion

For example, this is how a custom action to compose a new email could be added to a view.

```
var body: some View {
    ContentView()
        .accessibilityAction(named: Text("New Message")) {
            // Handle action
        }
}
```

