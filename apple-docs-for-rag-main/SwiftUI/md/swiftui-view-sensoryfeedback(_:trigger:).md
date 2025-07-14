

- SwiftUI
- View
-  sensoryFeedback(\_:trigger:) 

Instance Method

# sensoryFeedback(\_:trigger:)

Plays the specified `feedback` when the provided `trigger` value changes.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
func sensoryFeedback(
    _ feedback: SensoryFeedback,
    trigger: T
) -> some View where T : Equatable
```

## Parameters 

`feedback`  

Which type of feedback to play.

`trigger`  

A value to monitor for changes to determine when to play.

## Discussion

For example, you could play feedback when a state value changes:

```
struct MyView: View {
    @State private var showAccessory = false

    var body: some View {
        ContentView()
            .sensoryFeedback(.selection, trigger: showAccessory)
            .onLongPressGesture {
                showAccessory.toggle()
            }

        if showAccessory {
            AccessoryView()
        }
    }
}
```

## See Also

### Providing haptic feedback

func sensoryFeedback&lt;T>(trigger: T, (T, T) -> SensoryFeedback?) -> some View

Plays feedback when returned from the `feedback` closure after the provided `trigger` value changes.

func sensoryFeedback&lt;T>(SensoryFeedback, trigger: T, condition: (T, T) -> Bool) -> some View

Plays the specified `feedback` when the provided `trigger` value changes and the `condition` closure returns `true`.

struct SensoryFeedback

Represents a type of haptic and/or audio feedback that can be played.

