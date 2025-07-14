

- ManagedAppDistribution
- ManagedAppView
-  accessibilityAction(\_:\_:) 

Instance Method

# accessibilityAction(\_:\_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

ManagedAppDistributionSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func accessibilityAction(
    _ actionKind: AccessibilityActionKind = .default,
    _ handler: @escaping () -> Void
) -> ModifiedContent
```

## Discussion

For example, this is how a `.default` action to compose a new email could be added to a view.

```
var body: some View {
    ContentView()
        .accessibilityAction {
            // Handle action
        }
}
```

