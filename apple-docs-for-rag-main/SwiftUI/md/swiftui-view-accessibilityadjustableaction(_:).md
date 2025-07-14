

- SwiftUI
- View
-  accessibilityAdjustableAction(\_:) 

Instance Method

# accessibilityAdjustableAction(\_:)

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func accessibilityAdjustableAction(_ handler: @escaping (AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent
```

## Discussion

For example, this is how an adjustable action to navigate through pages could be added to a view.

```
var body: some View {
    PageControl()
        .accessibilityAdjustableAction { direction in
            switch direction {
            case .increment:
                // Go to next page
            case .decrement:
                // Go to previous page
            }
        }
}
```

## See Also

### Adding actions to views

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityActions&lt;Content>(() -> Content) -> some View

Adds multiple accessibility actions to the view.

func accessibilityAction(named:_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;Label>(action: () -> Void, label: () -> Label) -> some View

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;I, Label>(intent: I, label: () -> Label) -> some View

Adds an accessibility action labeled by the contents of `label` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction&lt;I>(AccessibilityActionKind, intent: I) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action representing `actionKind` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction(named:intent:)

Adds an accessibility action labeled `name` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityActions&lt;Content>(category: AccessibilityActionCategory, () -> Content) -> some View

Adds multiple accessibility actions to the view with a specific category. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action and are grouped by their category. When multiple action modifiers with an equal category are applied to the view, the actions are combined together.

struct AccessibilityActionKind

The structure that defines the kinds of available accessibility actions.

enum AccessibilityAdjustmentDirection

A directional indicator you use when making an accessibility adjustment.

struct AccessibilityActionCategory

Designates an accessibility action category that is provided and named by the system.

