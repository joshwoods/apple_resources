

- SwiftUI
- View
-  accessibilityActions(category:\_:) 

Instance Method

# accessibilityActions(category:\_:)

Adds multiple accessibility actions to the view with a specific category. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action and are grouped by their category. When multiple action modifiers with an equal category are applied to the view, the actions are combined together.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func accessibilityActions(
    category: AccessibilityActionCategory,
    @ViewBuilder _ content: () -> Content
) -> some View where Content : View
```

## Parameters 

`category`  

The category the accessibility actions are grouped by.

`content`  

The accessibility actions added to the view.

## Discussion

Var body: some View { EditorView() .accessibilityActions(category: .edit) { ForEach(editActions) { action in Button(action.title) { action() } } if hasTextSuggestions { Button(“Show Text Suggestions”) { presentTextSuggestions() } } } }

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

func accessibilityAdjustableAction((AccessibilityAdjustmentDirection) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility adjustable action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

func accessibilityScrollAction((Edge) -> Void) -> ModifiedContent&lt;Self, AccessibilityAttachmentModifier>

Adds an accessibility scroll action to the view. Actions allow assistive technologies, such as the VoiceOver, to interact with the view by invoking the action.

struct AccessibilityActionKind

The structure that defines the kinds of available accessibility actions.

enum AccessibilityAdjustmentDirection

A directional indicator you use when making an accessibility adjustment.

struct AccessibilityActionCategory

Designates an accessibility action category that is provided and named by the system.

