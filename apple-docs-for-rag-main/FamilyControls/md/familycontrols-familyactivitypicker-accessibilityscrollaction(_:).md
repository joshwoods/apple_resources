

- FamilyControls
- FamilyActivityPicker
-  accessibilityScrollAction(\_:) 

Instance Method

# accessibilityScrollAction(\_:)

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func accessibilityScrollAction(_ handler: @escaping (Edge) -> Void) -> ModifiedContent
```

## Discussion

For example, this is how a scroll action to trigger a refresh could be added to a view.

```
var body: some View {
    ScrollView {
        ContentView()
    }
    .accessibilityScrollAction { edge in
        if edge == .top {
            // Refresh content
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

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

