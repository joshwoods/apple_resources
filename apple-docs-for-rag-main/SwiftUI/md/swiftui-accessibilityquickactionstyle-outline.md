

- SwiftUI
- AccessibilityQuickActionStyle
-  outline 

Type Property

# outline

A presentation style that animates an outline around the view when the accessibility quick action is active.

watchOS 9.0+

``` source
static var outline: AccessibilityQuickActionOutlineStyle { get }
```

Available when `Self` is `AccessibilityQuickActionOutlineStyle`.

## Discussion

Use the contentShape(_:_:eoFill:) modifier to provide a shape for focusEffect if necessary.

The following example shows how to add an accessibilityQuickAction(style:content:) to play and pause music.

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

### Getting built-in menu styles

static var prompt: AccessibilityQuickActionPromptStyle

A presentation style that displays a prompt to the user when the accessibility quick action is active.

