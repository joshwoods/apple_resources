

- SwiftUI
- View
-  accessibilityAction(action:label:) 

Instance Method

# accessibilityAction(action:label:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

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

## See Also

### Adding actions to views

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityActions&lt;Content>(() -> Content) -> some View

Adds multiple accessibility actions to the view.

func accessibilityAction(named:_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;I, Label>(intent: I, label: () -> Label) -> some View

Adds an accessibility action labeled by the contents of `label` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction&lt;I>(AccessibilityActionKind, intent: I) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action representing `actionKind` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAction(named:intent:)

Adds an accessibility action labeled `name` to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action. When the action is performed, the `intent` will be invoked.

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

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

