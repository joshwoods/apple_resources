

- RealityKit
- RealityViewDefaultPlaceholder
-  accessibilityAction(named:\_:) 

Instance Method

# accessibilityAction(named:\_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

RealityKitSwiftUIiOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
nonisolated
func accessibilityAction(
    named name: S,
    _ handler: @escaping () -> Void
) -> ModifiedContent where S : StringProtocol
```

## Discussion

For example, this is how a custom action to compose a new email could be added to a view.

```
var body: some View {
    ContentView()
        .accessibilityAction(named: "New Message") {
            // Handle action
        }
}
```

