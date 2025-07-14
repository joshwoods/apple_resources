

- DeviceActivity
- DeviceActivityReport
-  accessibilityActions(category:\_:) 

Instance Method

# accessibilityActions(category:\_:)

Adds multiple accessibility actions to the view with a specific category. Actions allow assistive technologies, such as VoiceOver, to interact with the view by invoking the action and are grouped by their category. When multiple action modifiers with an equal category are applied to the view, the actions are combined together.

DeviceActivitySwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

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

