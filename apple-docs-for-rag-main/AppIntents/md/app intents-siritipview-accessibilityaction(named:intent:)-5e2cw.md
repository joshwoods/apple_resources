

- App Intents
- SiriTipView
-  accessibilityAction(named:intent:) 

Instance Method

# accessibilityAction(named:intent:)

Adds an accessibility action labeled with the localized representation of `nameKey` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

AppIntentsSwiftUIiOS 18.0+iPadOS 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityAction(
    named nameKey: LocalizedStringKey,
    intent: I
) -> ModifiedContent where I : AppIntent
```

