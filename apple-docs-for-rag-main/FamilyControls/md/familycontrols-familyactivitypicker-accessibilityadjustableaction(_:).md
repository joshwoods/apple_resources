

- FamilyControls
- FamilyActivityPicker
-  accessibilityAdjustableAction(\_:) 

Instance Method

# accessibilityAdjustableAction(\_:)

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

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

### Accessibility Actions

func accessibilityAction(AccessibilityActionKind, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;S>(named: S, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: Text, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction(named: LocalizedStringKey, () -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityAction&lt;Label>(action: () -> Void, label: () -> Label) -> some View

Adds an accessibility action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

