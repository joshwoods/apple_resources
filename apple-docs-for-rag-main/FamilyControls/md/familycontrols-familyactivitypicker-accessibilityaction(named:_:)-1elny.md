

- FamilyControls
- FamilyActivityPicker
-  accessibilityAction(named:\_:) 

Instance Method

# accessibilityAction(named:\_:)

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

FamilyControlsSwiftUIiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+watchOS 7.0+

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

## See Also

### Accessibility Actions

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: Text, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: LocalizedStringKey, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;Label>(action: () -> Void, label: () -> Label) -> some View

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

