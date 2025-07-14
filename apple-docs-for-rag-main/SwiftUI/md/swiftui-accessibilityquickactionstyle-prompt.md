

- SwiftUI
- AccessibilityQuickActionStyle
-  prompt 

Type Property

# prompt

A presentation style that displays a prompt to the user when the accessibility quick action is active.

watchOS 9.0+

``` source
static var prompt: AccessibilityQuickActionPromptStyle { get }
```

Available when `Self` is `AccessibilityQuickActionPromptStyle`.

## Discussion

The following example shows how to add an accessibilityQuickAction(style:content:) to pause and resume a workout.

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

## See Also

### Getting built-in menu styles

static var outline: AccessibilityQuickActionOutlineStyle

A presentation style that animates an outline around the view when the accessibility quick action is active.

