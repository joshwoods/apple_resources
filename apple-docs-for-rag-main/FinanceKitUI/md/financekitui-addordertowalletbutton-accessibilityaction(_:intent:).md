

- FinanceKitUI
- AddOrderToWalletButton
-  accessibilityAction(\_:intent:) 

Instance Method

# accessibilityAction(\_:intent:)

Adds an accessibility action representing `actionKind` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

FinanceKitUISwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityAction(
    _ actionKind: AccessibilityActionKind = .default,
    intent: I
) -> ModifiedContent where I : AppIntent
```

