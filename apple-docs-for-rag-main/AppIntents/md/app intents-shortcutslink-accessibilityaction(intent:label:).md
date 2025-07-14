

- App Intents
- ShortcutsLink
-  accessibilityAction(intent:label:) 

Instance Method

# accessibilityAction(intent:label:)

Adds an accessibility action labeled by the contents of `label` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

AppIntentsSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityAction(
    intent: I,
    @ViewBuilder label: () -> Label
) -> some View where I : AppIntent, Label : View
```

