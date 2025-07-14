

- SwiftUI
- View
-  accessibilityQuickAction(style:content:) 

Instance Method

# accessibilityQuickAction(style:content:)

Adds a quick action to be shown by the system when active.

watchOS 9.0+

``` source
nonisolated
func accessibilityQuickAction(
    style: Style,
    @ViewBuilder content: () -> Content
) -> some View where Style : AccessibilityQuickActionStyle, Content : View
```

## Discussion

The quick action will automatically become active when the view appears. If the view is disabled, the action will defer becoming active until the view is no longer disabled.

The following example shows how to add a quick action to pause and resume a workout, with the prompt style.

```
@State private var isPaused = false

var body: some View {
    WorkoutView(isPaused: $isPaused)
        .accessibilityQuickAction(style: .prompt) {
            Button(isPaused ? "Resume" : "Pause") {
                isPaused.toggle()
            }
        }
}
```

The following example shows how to add a quick action to play and pause music, with the outline style.

```
@State private var isPlaying = false

var body: some View {
    PlayButton(isPlaying: $isPlaying)
        .contentShape(.focusEffect, Circle())
        .accessibilityQuickAction(style: .outline) {
            Button(isPlaying ? "Pause" : "Play") {
                isPlaying.toggle()
            }
        }
}
```

## See Also

### Offering Quick Actions to people

func accessibilityQuickAction&lt;Style, Content>(style: Style, isActive: Binding&lt;Bool>, content: () -> Content) -> some View

Adds a quick action to be shown by the system when active.

protocol AccessibilityQuickActionStyle

A type that describes the presentation style of an accessibility quick action.

